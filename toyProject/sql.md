
## 멤버

CREATE TABLE member(
member_no NUMBER PRIMARY KEY,
member_id VARCHAR2(30) NOT NULL UNIQUE,
member_pw VARCHAR2(30) NOT NULL,
member_email VARCHAR2(30) NOT NULL,
member_address VARCHAR2(30) NOT NULL,
member_grade VARCHAR2(30) DEFAULT '일반' NOT NULL CHECK(member_grade IN('일반', '관리자'))
);
