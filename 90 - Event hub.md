
## Deep dive

https://www.youtube.com/watch?v=358TuU88Nvg&t=3517s


<img width="1880" height="1063" alt="image" src="https://github.com/user-attachments/assets/43416009-c01a-4e6e-a486-d853503dc528" />




<img width="809" height="429" alt="image" src="https://github.com/user-attachments/assets/3b1ee8a1-f816-4fad-abcb-2961b8c79010" />

# Error

<img width="1019" height="153" alt="image" src="https://github.com/user-attachments/assets/dffcb0b2-b615-46a7-a6b9-f40453c82375" />

# or you can see problem on chart throthling  
if you use Kafka protocol you will not see this error

if you have problem wiht thotling consider  - premium or dedicated
<img width="868" height="567" alt="image" src="https://github.com/user-attachments/assets/549def3d-0d9d-4130-b1ab-37dea61806c8" />



you may encounter when you use event hubs heavily. The most
common reason for getting throttling errors is not having
sufficient capacity allocated for your event hubs namespace.
For example, if you are using EVENTHUBS standard tier and you
don't have sufficient throughput units to handle the ingress data
load, then your workload will get totaled. Also in real
situations where you are workload is skewed towards 1
partition you may also observe throttling errors. You can


# To detect 
ou can look for throttle request  metric to determine the count of throttling.
Also, you can detect throttling errors from the client

#  Mitigate
## 1
You can resolve throttling errors that you encounter in event Hub standard tier by increasing the throughput units
## 2
 higher tier such dedicated or premium
## 3
or we can see issue in particions if you have only one



