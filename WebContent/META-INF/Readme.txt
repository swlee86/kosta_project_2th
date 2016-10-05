CREATE table notice(  --공지사항용 게시판
idx number constraint pk_notice_indx Primary Key, -- 글번호(중복되면 안되기 때문에 Pk 지정
writer VARCHAR2(30) NOT NULL , --글쓴이 (회원전용: 로그인한 ID , 별칭     비회원용: 입력값 )
subject VARCHAR2(50) NOT NULL, --글제목
content VARCHAR2(100) NOT NULL, --글내용
writedate DATE DEFAULT SYSDATE, -- 작성일
filename VARCHAR2(200),  --파일명 (test.txt)
filesize NUMBER              --파일크기(byte)
);