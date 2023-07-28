# Create EC2 Instance

In this post we will learn to create an EC2 Instance.
For full tutorial follow [this](https://www.youtube.com/watch?v=Dc0t4LDOySY&list=PLdpzxOOAlwvLNOxX0RfndiYSt1Le9azze&index=4&pp=iAQB) video 

1.  Signup/Login to the console. Follow [this](console.aws.amazon.com/) link

2. On the search bar search `ec2` and click on the 1st option or url with text **ec2** _i.e_ ec2

3. Click on the **red colored rectangle** mentioned below
	![Instance Creation](https://imgur.com/wXFU4jU.png)
4. Click on the **Launch Instance**
	<details>
	<summary>IMG</summary>

	![](https://imgur.com/utMETuI.png)

	</details>

5. Fill the details
- Name -> [any name](https://imgur.com/7WPpqrQ.png) of the instance of your wish. 
	
	![Name of instance](https://imgur.com/7WPpqrQ.png)
- OS Image -> the OS you want for your remote server. 
	- [recommended](https://imgur.com/XUUsFlB.png): **ubuntu**
	
	
		![OS Image](https://imgur.com/XUUsFlB.png)
- Instance type -> This include the combinations of cpu, storage, memeory, networking capacity.
	- You choose as per your requiremtns.
	- [recommended](https://imgur.com/mErPeiI.png): **t2.micro** as this is included in free tire
			![Instance Type](https://imgur.com/mErPeiI.png)
- Key Pair login 
	- This will be used for you to login in your aws instance

	- Create new one or choose existing
	- Creating new  key pair
		- Click on [create new](https://imgur.com/PCLh5Ph.png)
		- Give **[any name and leave rest unchanged](https://imgur.com/OuJXoOj.png)** and then click on the **create key pair**. Download it to any location
		- Once the above steps are done, click on the [reload icon](https://imgur.com/wyh3sdT.png)
		- Then, choose the [key](https://imgur.com/rh0pDyV.png) from the dropdown
	- User existing one 
		- click on the [reload icon](https://imgur.com/wyh3sdT.png)
		- Then, choose the [key](https://imgur.com/rh0pDyV.png) from the dropdown
- **Leave rest as it is.**

6) Click on the **Launch Instance.**

7) After all this, [Click on](https://imgur.com/tXyNKnl.png) on the Successfully initiated launch of instance **i-xXXxXXxx** 
	-	i-xXXxXXxx -> your instance ID. Every instance will have its own ID
	
	![Click on instance id](https://imgur.com/tXyNKnl.png)

8) Probably your screen should be like [this](https://imgur.com/js5Fs18.png)

	![Screen](https://imgur.com/js5Fs18.png)

9) Click on the **[Instance ID](https://imgur.com/3lCZAah.png)**

	![Instance ID](https://imgur.com/3lCZAah.png)

10) Copy the **[Public Ip Address](https://imgur.com/0ZKfYXi.png)**
	![Ip Address](https://imgur.com/0ZKfYXi.png)

10) Open your [favourate terminal](https://imgur.com/yYOhmnC.png) 
	- Goto the path where the key pair file [was](https://imgur.com/gOi8lxB.png) downloaded.
	- use command `chmod 400 filename.pem`, as like [this](https://imgur.com/JedyEOY.png).
		- If you are interested behind the scene of `chmod 400` follow [this]().
12.   Type the commad 
	`ssh -i /path/of/key/downloaded ubuntu@public.ip.address.`
	![Command](https://imgur.com/50FXasm.png)
	
- Click yes and **enjoy**

![Final Output](https://imgur.com/1ex8kJQ.png)
	 
