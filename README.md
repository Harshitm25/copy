Query 1.
select * from student where sem=2 and branchid in
(select branchid from branch where bname='mca')
Query 2.
select * from student where usn not in (select usn from borrow);

Query 3.
select student.usn ,student.name,branch.bname, book.bname, aname, borrowdate from student ,
branch, book, author, borrow where student.usn=borrow.usn and borrow.bookid=book.bookid and
book.authorid =author.authorid and student.branchid=branch.branchid and student.sem=2 and
branch.bname='mca';
Query 4.
select count(*) , authorid from book group by authorid;
Query 5.
select * from student where usn in ( select usn from borrow group by usn having count(usn) >=2);
Query 6.
select * from student s where exists (select br.usn from borrow br join book bk on br.bookid=bk.bookid
where br.usn=s.usn group by usn having count(distinct authorid)>1);
Query 7.
select bname from book order by bname desc;
Query 8.
select * from student s where exists (select usn , publisher from borrow join book on
borrow.bookid=book.bookid where s.usn=borrow.usn group by usn having count(distinct publisher)=1);


3)Query 1 :
Select pname, tname, age from player p, team t where p.tid=t.tid and age =(select min(age) from
player);
Query 2:
select * from stadium where sid in
(select sid from match group by sid having count(sid) = (select max(count(sid)) from match group by
sid))
Query 3:
select * from player where pid not in ( select captain_pid from team) and pid in (select man_of_match
from match group by man_of_match having count(man_of_match)=2);
Query 4:
select * from team where tid in (select winning_team_id from match group by winning_team_id having
count(winning_team_id)= (select max(count(winning_team_id))from match group by
winning_team_id))
Query 5
select tname from team where tid in (
select winning_team_id from match group
by(winning_team_id,sid)
having count(*) in (select count(winning_team_id)from match group by winning_team_id)).

4)Query 1:
select state from tourist_place group by state having
count(state)=(select max(count(state)) from tourist_place group by state);
query 2:
select * from tourist_place where tpid in (select tpid from visits group by tpid having count(tpid)=
(select max(count(tpid)) from visits group by tpid));
query 3:
select * from tourist t where t.tid in
(select tid from visits join tourist_place on
visits.tpid=tourist_place.tpid where state='karnataka'group by tid having count(state) in (select count(state) from tourist_place where state='karnataka'));
query 4:
select * from tourist t where t.tid in (select tid from visits join tourist_place on
visits.tpid=tourist_place.tpid
group by tid having count(distinct state)
in (select count(distinct state ) from tourist_place) );
query 5:
select * from tourist_place where tpid in (
select tpid from visits join tourist on visits.tid=tourist.tid group by tpid having count(distinct country)=
(select count(distinct country) from tourist));

5)Query 1:
select * from candidates where cand_id in (select cand_id from contest join constituency on
contest.cons_id=constituency.cons_id group by cand_id having count(distinct(csstate))>1);
Query 2:
select csstate from constituency group by csstate having count(csstate) in (select max(count(csstate))
from constituency group by csstate);

query 3:
create or replace procedure agechecking ( id in number,age in number)
as
BEGIN
if age>18 then
insert into voter(vid,vage) values (id,age);
else
dbms_output.put_line('age should be high');
end if;
end agechecking;
/
Procedure created.
SQL> set serveroutput on;
SQL> exec agechecking (25,21);
PL/SQL procedure successfully completed. // row inserted
SQL> exec agechecking (20,15);
age should be high //Message displayed as age is less than or equal to 18 PL/SQL procedure
successfully completed.
query 4:
create or replace procedure display_count
(
const_id in number
)
as
vid constituency.cons_id % type;
begin
select no_of_voters into vid from constituency where cons_id = const_id and rownum = 1;
dbms_output.put_line ( 'total voters are: ' || vid);
end;
/
Procedure created.
SQL> select * from constituency;
CONS_ID CSNAME CSSTATE NO_OF_VOTERS ---------- -------------------- -------------------- ------------
111 rajajinagar karnataka 2 222 ramnagar kerala 1
SQL> exec display_count(111);
total voters are: 2
Query 5:
create or replace trigger count
after insert on voter
for each row
begin
CMRIT
update constituency
set no_of_voters = no_of_voters + 1
where cons_id=:new.cons_id;
end count;
/
Trigger created.
SQL> set serveroutput on;
SQL> select * from constituency;






