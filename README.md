## Web Spring Boot

-----------------------------------------------------------------
11.30
test Procedure
		
DELIMITER $$

CREATE PROCEDURE testDataInsert()
BEGIN
    DECLARE i INT DEFAULT 1;

    WHILE i <= 120 DO
        INSERT INTO board(title, content)
          VALUES(concat('제목',i), concat('내용',i));
        SET i = i + 1;
    END WHILE;
END$$

DELIMITER ;

-------------------------------------------------------------------
11.29

1. 게시판 작성구현

2. DB연동 

3. 게시글 작성 시 DB table 에 insert

-------------------------------------------------------------------

1. bootstrap 템플릿사용 main demo 구성
	index.html / manager.html/ styles.css / scripts.js / images

2. 관리자 버튼 클릭시 관리자 페이지로 이동구현
	-> 관리자로 로그인시 관리자 페이지버튼 생성으로 변경 예정.  

	-> 관리자 페이지 템플릿 적용 예정.   

3. DB연동 예정 



