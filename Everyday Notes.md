##Notes for Calibrated Tool Service 

##What Service does what 

####getCertSystemCerts
Input

```html
	<arg0>
   		<!--Optional:-->
        <avlFromDt>?</avlFromDt>
        <!--Optional:-->
        <discFromDt>?</discFromDt>
        <hasParent>?</hasParent>
        <!--Optional:-->
        <id>?</id>
        <!--Optional:-->
        <name>?</name>
        <!--Optional:-->
        <parentCertId>?</parentCertId>
        <!--Optional:-->
        <version>?</version>
	</arg0>
```

What i send 

```html
	<arg0>
            <!--Optional:-->
            <id>*</id>
            <!--Optional:-->
            <name>*</name>            
         </arg0>

```

```java

public List<Certification> listAllByEsiCertId(String certificationId) throws SQLException{ 
		conn = getConnection();
		if(!certificationId.contains("*")){
			certificationId += "*";
		}
		certificationId = certificationId.replace('*', '%').toUpperCase();
		List<Certification> certList = new ArrayList<Certification>();
		try{
			ps = conn.prepareStatement(LIST_BY_ESI_CERT_ID);
			int i = 1; 
			ps.setString(i++, certificationId);
			rs = ps.executeQuery(); 
			while(rs.next()){
				Certification certification = new Certification();
				certification.setCertificationId(rs.getString(CERTIFICATION_ID));
				certification.setCertificationDsc(rs.getString(CERTIFICATION_DSC));
				certList.add(certification);
			}
				}finally{
			releaseAll();			
		}return certList;	
	}
```


##Scatch pad for Wednesday
#####no data for test 
	ALL NEED THIS 	
	- PartAttributeSuite
		- getPartAttributeByPartId
		
	- add revenue service to test and only test 
		
		
```C++
	
	arr[0] = 12; 
	arr[1] = 42;
	
	
 	
```
	
		
