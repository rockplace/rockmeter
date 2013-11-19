rockmeter
=========

Description
Rockmeter is performance test solution for middleware.
There are scripts capture application and web-based test application using jmeter opensource engine.
so users can do WAS performance test using web-interface easily.



Features
- Web based performance test suite.
- Auto scripting support
- Web based reporting support include file export.


# Public beta version is released.
- Last weekend-2013-11-15-, Public beta version was released.
- Everybody can test the rockmeter which is web based application on Jmeter.
- If you have a question, please send e-mail to me. 
- E-mail address is rockmeter@rockplace.co.kr.
- You can download on sourceforge.net site-https://sourceforge.net/projects/rockmeter-. 
- We will upload the rockmeter source file on the site as soon as possible.

# Packages
 in rockMeter.zip
  Control Tower - rockmeter.war
  Control Tower Database schema - rockmeter_20131114.sql
  Jmeter for agent - rockmeter_agent_jmeter.tar.gz
  Agent for admin - rockmeter_agent.war

# Installation
 - Control Tower
  1. Install Tomcat 7 in your machine.
  2. Install MySQL 5.5 in your machine.
  3. Insert database schema into your MySQL server.
     $ mysql -uroot -p rockmeter < rockmeter_20131114.sql
  4. Put rockmeter.war into %TOMCAT_HOME%/webapps
  5. Config your database information into %TOMCAT_HOME%/webapps/rockmeter/WEB-INF/properties/jdbc.properties
  6. Start Tomcat.
  7. Default user admin/admin..

 - Jmeter for agent
  1. Extract rockmeter_agent_jmeter.tar.gz into /usr/local/jmeter.
  2. Set owner tomcat user.
     $ chown -R tomcat:tomcat /usr/local/jmeter/
  3. Check permission 777 of scripts directory (/usr/local/jmeter/scripts/)
  4. Run agent using run_agent.sh script. (/usr/local/jmeter_agent)

 - Agent for admin
  1. Install Tomcat 7 in your machine.
  2. Install MySQL 5.5 in your machine.
  3. Put rockmeter.war into %TOMCAT_HOME%/webapps
  4. Config your database information into %TOMCAT_HOME%/webapps/rockmeter/WEB-INF/properties/jdbc.properties
  5. Start Tomcat.
