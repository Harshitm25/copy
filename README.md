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


2)
