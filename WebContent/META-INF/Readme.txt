CREATE table notice(  --�������׿� �Խ���
idx number constraint pk_notice_indx Primary Key, -- �۹�ȣ(�ߺ��Ǹ� �ȵǱ� ������ Pk ����
writer VARCHAR2(30) NOT NULL , --�۾��� (ȸ������: �α����� ID , ��Ī     ��ȸ����: �Է°� )
subject VARCHAR2(50) NOT NULL, --������
content VARCHAR2(100) NOT NULL, --�۳���
writedate DATE DEFAULT SYSDATE, -- �ۼ���
filename VARCHAR2(200),  --���ϸ� (test.txt)
filesize NUMBER              --����ũ��(byte)
);