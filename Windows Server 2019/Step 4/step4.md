# Performance Tuning and Security Best Practices

## Performance Monitoring
We will be using two tools there :

- `Performance monitor (Perfmon)` : it permits to have the overview of performance from mostly whatever could exist in your computer.
  You can open the tool via typing his name on the search bar.
  ffffffffffff


  Click on the plus button to add other characteristics. Click on the add sign and add as shown :
  
<img width="738" alt="image" src="https://github.com/user-attachments/assets/3b41a2d9-eae0-4727-8b2f-11eaaf60d1a1">

Another method is to use the `Data Collector Sets`.
To create one :
- Right Click on User Defined :
<img width="738" alt="image" src="https://github.com/user-attachments/assets/1b8d3bed-af1f-4f2d-9003-f31216ea4ef1">
fffffff
- Name it as you like :
  
<img width="740" alt="image" src="https://github.com/user-attachments/assets/b008af6b-ff16-4a10-aefc-1de2fb0788b6">

<img width="742" alt="image" src="https://github.com/user-attachments/assets/38e7a0a0-c25e-4c63-86a9-2810b30e4479">

Add the counters as previously and finish.
Now you need to launch the Collector :
![image](https://github.com/user-attachments/assets/bf88df78-c785-4ee9-a050-a5303bb84934)
 Wait for 10 mins and stop it :
 ![image](https://github.com/user-attachments/assets/0819a042-c155-4559-8503-153f14bac794)
 
Now to open it, we can go to the performance monitor and we will import the collected file as follow :
![image](https://github.com/user-attachments/assets/f4254826-7df6-43a1-8b31-f8a0d72fc5f9)

And that's it, you have all the previously choosen counters displayed in the window.
![image](https://github.com/user-attachments/assets/47d136c9-b39d-4fd3-8ffb-b6f736fab99a)


- `Ressource monitor` : this tool helps to more get an depth view on system ressources consumption such as ( cpu, memory and network)
  You can open the tool via typing his name on the search bar.
<img width="587" alt="Screenshot 2024-08-24 150655" src="https://github.com/user-attachments/assets/0834fa7c-3012-4f73-b855-dfdd65bbc846">

  Open it and you can explore the window.
ffffffffffff

<img width="578" alt="Screenshot 2024-08-24 145912" src="https://github.com/user-attachments/assets/a24b427f-964b-451e-bbfc-b8c76a4c3bc5">

<img width="588" alt="Screenshot 2024-08-24 150131" src="https://github.com/user-attachments/assets/4249519b-06db-407b-820a-74c9f5ddf28e">


To focus on a specific process, just tick it and you will see a dfferent color representating the process (a yellow color as shown in the screenshot)

<img width="587" alt="image" src="https://github.com/user-attachments/assets/ab1eb9de-d062-4ae5-a655-9f962d3411c5">

You can explore the diverse tabs to see the consumption by memory, network and processes...Just give it a try

