

# Arweaver📨

Arweaver is a protocol that will send an email to a web2 email account when an on-chain transaction occurs involving a user’s wallet address. 

![Home Page](https://i.ibb.co/mch1M20/Mac-Book-Pro-14-7.png)
[](https://arweaver.xyz)<center>https://arweaver.xyz</center>

> 🔴**IMPORTANT**🔴 
> Create a new account if your mail limit exceeds.

# Get Started

The product contains two code bases, Server to serve the Client and also polls for a recent blocks, a GUI code base. Database is handled by [kwil](https://kwil.com/), a SQL database for web3.

1. [Server](https://github.com/leostelon/arweaver-server)
2. [Client](https://github.com/leostelon/arweaver-client)

**Website**

[arweaver.xyz](https://arweaver.xyz/)

**API**

[API Arweaver](https://api.arweaver.xyz/)

# Accomplishments/Milestones

 - Created a simple poling server using node.js..
 - Enabled [Othent](https://othent.io/) for easy onboarding for Web2 users.
 - Migrated from Amazon SES to Mailgun for mailing solution.

# Technology
 - **Node.js server** with Express.js.
 - Database, **Kwil &  MongoDB**. [[kwil.com]](https://kwil.xyz/)
- **ArConnect** is the secure gateway to the leading platforms in the growing Arweave ecosystem, [[know more]](https://www.arconnect.io/)
- **Othent** allows web3 dApps and protocols to seamlessly access web2 users, [[know more]](https://othent.io/)
- React.js for client.

**Overview of polling server**

![Home Page](https://i.ibb.co/D58M5B1/Screenshot-22.png)
 
[Full code here↗️](https://github.com/leostelon/arweaver-server/blob/main/src/subscriber.js)

Follow the below steps to run it locally.

## Server⚙️
> ⚠️ Make sure you have installed Bacalhau Client. [Know More](https://docs.bacalhau.org/getting-started/installation)

1. Clone Repo.
> $ git clone https://github.com/leostelon/arweaver-server arweaver-server
>  $ cd arweaver-server
2. Add the .env file in the root directory. Add the below variables and replace them with your tokens, respectively.

    	  INFURA_ID= < infura-token > [Know More](https://www.infura.io/)
		  ETH_PVT_KEY= < eth-pvt-key >
	      MAILGUN_API_KEY= < mailgun-api-key >[Know More](https://mailgun.com/)

3. Run server!
#### Run independently
> $ npm run start



## Client💻

1. Clone Repo.
> $ git clone https://github.com/leostelon/kissingface-client kissingface-client
>  $ cd kissingface-client
2. Add the .env file in the root directory. Replace the value accordingly.

		  REACT_APP_SERVER_URL=http://localhost:3000
		  REACT_APP_API_ID=< othent-api-key > [Know More](https://othent.io/)
	  
4. Run the client!
> $ npm run start

Note: It may prompt to run on a different port, hit enter.

## What next?👨‍💻
 - [x] Polling Server
 - [x] Mailgun
 - [x] Rate limit
 - [ ] Convert completely to Kwil.
