# ytrued
for ytrued

create table userinfo(
    id varchar2(20) primary key,
    pw varchar2(16) not null,
    name varchar2(12) not null,
    phone varchar2(20) not null,
    usertype number not null
);

insert into userinfo values('admin' , 'blabla', '쿠팡맨' , 'phonenumber', 0);

ROLLBACK;
commit;

DROP TABLE userinfo;

select * from userinfo;


<Resource auth="Container" driverClassName="oracle.jdbc.OracleDriver" maxIdle="10" maxTotal="20" maxWaitMillis="-1" name="jdbc/myoracle" password="hong" type="javax.sql.DataSource" url="jdbc:oracle:thin:@127.0.0.1:1521:myoracle" username="ora_user"/>
      </Context>
