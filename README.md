# demo04 구현 사항
SpringBoot 

Restful API 
  - Create
    putCustomer(Customer customer)
  - Update
    postCustomer(Customer customer)
  - Delete
    deleteCustomer(int id)
  - Read
    getCustomer(int id)
    getCustomer(String name)
    searchCustomer(String name)
    getCustomerList()
  
h2 
  - Local Console 접속
    http://localhost:8080/h2-console/
  
jpa hibernate
  - Repository 
    findByName(String name);
	  findByNameLike(String Name);
	  findByNameAndAddress(String Name, String Address);
	  findByNameAndAddressOrderByNameDesc(String Name, String Address);
	  @Query(value="select * from Customer where name=?1 and address=?2", nativeQuery=true)
	  findVipList(String value1, String value2);
