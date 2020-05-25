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
