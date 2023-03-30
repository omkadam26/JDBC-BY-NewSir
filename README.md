# JDBC-BY-NewSir
JDBC Started

JDBC API

Java Application

DB Server
      To store data permanently 
      
      in file also we are able to store data and we can use the data .
      we can store data in database in table format or in relation.
      we can efficently fetch the data.
      and main issue is security
      java developer wants to store data store permanently 
      
      
      JDBC API
      API 
          is way to interact the one program with another programm.
          here java application is one program and another is database. 
          jdbc api provides predife classes, methods,
          package java.sql  ==> it contains jdbc related content.
          
          
          jdbc to store data parmantley and persistenly
          if i want to transfer data from one application to another application.
          driver is used to transfer the one computer to another
          driver:
                  how i store data from one application with another.
                        os needs driver.
                        
                        
           driver : is set of instructions which is used to communcate between them.
           
           load the driver.
           
           
         ----------------------------------------------------------------------------
           
           
           //Notes given by Sir
      
           1. Jdbc API(java Database Connectivity  Application programming interface) 
                which provices the way to communicate with one program with another program.
           2. The main purpose  of JDBC api is to store the Applications data permanently to the database server
               (oracle,mysql,postgre,etc.)
           3. Data server provides way to organize our data , so that data can be easily and efficiently 
              access,remove or update.
           5. To communicate Java Application  with database we need drivers.
                   Driver: is a software or program on the set of instructions which expose the functionality of another software on hardware
           6. There are 4 types of drivers are available:
                                          1.Type1 Driver or JDBC-ODBC(Open database Connectivity) bridge driver.
                                                it not entirely  not written in java language.
                                          2.Type2 Driver or Native API driver
                                          3.Type3 Driver Network protocol driver.
                                          4.Type4 Driver or Thin Driver.
                                          
                                          #Type1 
                                          JDBC API                JDBC-ODBC               ODBC Function            Vendor Specific
                                          |           ==>       bridge Driver   ==>           Call         ==>           Libs         ==> Database
                                          |
                                          V 
                                          Applications 
                                          
                                          
                                          1.  In case of  Type1 Driver ,The JDBC method calls converted into ODBC Function call
                                          2.  Each and every client machine required to install vendor specific libraries 
                                          3.  It degrade The Performance due to so many conversion
                                          4.  Oracle does not support type1 Drivers from JDK1.8 version.
                                          
                                          
                                          #Type2 Drivers
                                          
                                          JDBC API                Native APi               Vendor Specific
                                          /\           ==>          Driver      ==>          Libs              ==> Database
                                          |
                                          V 
                                          Applications 
                                          
                                                In this case it upgrades performace then Type1 Driver.
                                                1.    We must need to install native driver in each and every client machine.
                                                2.    we must to need to include vendor specific in every client machine.
                                                
                                          
                                          #Type3 Driver
                                          
                                          JDBC API                Network protocol              Middletier On Application
                                          /\           ==>          Driven Driver  ==>                 Server                 ==> Database
                                          |
                                          V 
                                          Applications 
                                          
                                              #Type3 Driver on Network Protocol Driver.
                                                      1.It Required Network support to communicate with database.
                                                      2.    we need to vendor specific middletier  code to communicate with database.
                                                      
                                         #Type4 Driver or Thin Driver.
                                          
                                          JDBC API                        Thin 
                                          /\           ==>               Server                 ==> Database
                                          |
                                          V 
                                          Applications  
                                          
                                          In Type4 we don't  need any conversion. dont need any middletier specific code.
                                          it is purely developed written in java language.
                                          
           
                
                
      
      
