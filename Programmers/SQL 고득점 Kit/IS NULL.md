## [이름이 없는 동물의 아이디](https://school.programmers.co.kr/learn/courses/30/lessons/59039)
~~~sql
SELECT 
    ANIMAL_ID
FROM ANIMAL_INS
WHERE NAME IS NULL
ORDER BY ANIMAL_ID
~~~

## [이름이 있는 동물의 아이디](https://school.programmers.co.kr/learn/courses/30/lessons/59407)
~~~sql
SELECT 
    ANIMAL_ID 
FROM ANIMAL_INS
WHERE NAME IS NOT NULL
ORDER BY ANIMAL_ID
~~~

## [NULL 처리하기](https://school.programmers.co.kr/learn/courses/30/lessons/59410)
~~~sql
SELECT
    ANIMAL_TYPE,
    IFNULL(NAME,'No name'),
    SEX_UPON_INTAKE
FROM ANIMAL_INS
ORDER BY ANIMAL_ID
~~~
