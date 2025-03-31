<h1>Wireshark- Protocol Filter</h1>


<h2>Description</h2>
Answering questions using filters

<h2>Questions</h2>

- <b>What is the number of IP packets?</b>
- <b>What is the number of packets with a "TTL value less than 10"?</b>
- <b>What is the number of packets which uses "TCP port 4444"?</b>
- <b>What is the number of "HTTP GET" requests sent to port "80"?</b>
- <b>What is the number of "type A DNS Queries"?</b>


<h2>Languages and Utilities Used</h2>

- <b>Wireshark</b> 


<h2>Environments Used </h2>

- <b>TryHackMe VM</b> 

<h2>Program walk-through</h2>

<b>Answer the question below <br/>

What is the number of IP packets?

<p align="center">
Starting at the Filter Bar, type in ip and press enter. It will filter pretty quickly. Look at the bottom right of the Wireshark window. You are looking for the word Displayed. The numbers to the right of Displayed, is the answer: <br/>
<img width="1440" alt="Screenshot 2025-03-31 at 3 16 51 PM" src="https://github.com/user-attachments/assets/f749e22d-53bd-4229-8d78-56fa9f2958f4" />



<br />
<br />
Answer is 81420: <br/>





<h2>Program walk-through</h2>

<b>Answer the question below <br/>
What is the number of packets with a "TTL value less than 10"?

<p align="center">
Go to the Filter Bar. The filter will be ip.ttl <10, and will look for IPv4 address that have a time to live of less than 10. After you have entered in this filter, press enter to use it. You should only have the Packets that match the filter remaining. Go back down to Displayed in the bottom right of the Wireshark window. The number to the right is the answer to this question: <br/>
<img width="1440" alt="Screenshot 2025-03-31 at 3 32 36 PM" src="https://github.com/user-attachments/assets/5ee20152-d37b-41a6-846a-16302901db40" />



<br />
<br />
Answer is 66: <br/>






<h2>Program walk-through</h2>

<b>Answer the question below <br/>
What is the number of packets which uses "TCP port 4444"?


<p align="center">
Go to the Filter Bar. The filter to use is tcp.port == 4444. Type this into the Filter Bar and press enter. Go to Displayed in the bottom right of the Wireshark window. The number to the right is the answer to this question.: <br/>
<img width="1440" alt="Screenshot 2025-03-31 at 3 39 31 PM" src="https://github.com/user-attachments/assets/6f673522-f184-4cb6-9400-10fba98e36b4" />



<br />
<br />
Answer is 632: <br/>





<h2>Program walk-through</h2>

<b>Answer the question below <br/>
What is the number of "HTTP GET" requests sent to port "80"?

<p align="center">
Go to the Filter Bar. Enter the filter, http.request.method == GET and tcp.port == 80 and press enter. Go back down to Displayed in the bottom right of the Wireshark window. The number to the right is the answer to this question: <br/>
<img width="1440" alt="Screenshot 2025-03-31 at 3 47 33 PM" src="https://github.com/user-attachments/assets/298a83ad-c7e4-4ba9-b588-6d48b593aba9" />



<br />
<br />
Answer is 527: <br/>






<h2>Program walk-through</h2>

<b>Answer the question below <br/>
What is the number of "type A DNS Queries"?


<p align="center">
Start typing in the Filter Bar, dns.a. Press enter to use the filter. Go to Displayed in the bottom right of the Wireshark window. The number to the right is the answer to this question: <br/>
<img width="1440" alt="Screenshot 2025-03-31 at 3 54 08 PM" src="https://github.com/user-attachments/assets/94b8240f-f059-4d93-a3ad-08d607983b18" />



<br />
<br />
Answer is 51: <br/>


