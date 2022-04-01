# jpashop

DDL - Data Definition Language : CREATE, ALTER, DROP, TRUNCATE <br>
DML - Data Manipulation Language : SELECT, INSERT, UPDATE, DELETE<br>
DCL - Data Control Language : GRANT, REVOKE<br>

@Entity - managed by JPA, act like an Table : required default constructor<br>
hibernate.hbm2ddl.auto - create, creat-drop, update, validate, none <br>

@Column - Mapping to table's column <br>
@Enumerated - Mapping to Java's Enum type <br>
@Lob - Mapping to Blob, Clob <br>
• CLOB: String, char[], java.sql.CLOB 
• BLOB: byte[], java.sql. BLOB 

@Id, @GeneratedValue: IDENTITY: MYSQL ,  SEQUENCE: ORACLE, AUTO - @SequenceGenerator is needed <br>

• AUTO_ INCREMENT는 데이터베이스에 INSERT SQL을 실행한 이후에 ID 값을 알 수 있음
• IDENTITY 전략은 em.persist() 시점에 즉시 INSERT SQL 실행하고 DB에서 식별자를 조회

allocationSize option for @SequenceGenerator


* Team Id for a new member is handled by member's class setter. -> It's not a good practice in terms of Object Oriented<br>
![image](https://user-images.githubusercontent.com/76544061/161160369-06ad46e1-1f98-4c3c-a002-1d3f0c4c219b.png)

![image](https://user-images.githubusercontent.com/76544061/161160174-5f9df8b2-1da8-4f80-ae4e-d3a21b1e8561.png)

* For good practice, use object as reference - Object Oriented Modeling! 
* ![image](https://user-images.githubusercontent.com/76544061/161160506-6f6d748b-6db1-41ee-9b3d-0ae7b8afacb0.png)
