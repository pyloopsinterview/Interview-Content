## Q1. You done the tap-to-pay start with the python previously?

Ans: Yes, I’ve worked on the **Tap-to-Pay** feature as part of a **payment integration module** using **Python** for backend processing.

We implemented this using **NFC (Near Field Communication)** technology, where the frontend or mobile device captures the card token through a secure NFC reader. The Python backend, built using **Flask**, handled the secure **tokenization, authorization, and transaction processing**.

We integrated with **payment gateways** like **Stripe** and **Mastercard’s Tap-on-Phone APIs** to process the transactions. The card details were **never stored directly** — we only worked with **tokenized card data** to comply with **PCI-DSS security standards**.

## Q2. In which project you had worked on tap-to-pay?

Ans: I worked on the **Tap-to-Pay** feature during my time at **Flagstar Bank**.  
Our goal was to enable **contactless payments** through mobile devices, similar to how **Apple Pay** or **Google Pay** work.

In this project, my primary responsibility was to develop the **Python backend services** that handled **digital wallet management**, **card tokenization**, and **transaction authorization**.

We built secure **REST APIs** using **Flask** that communicated with **payment processors** like **Mastercard** and **Visa** through their **tokenization and authorization APIs**.  
The entire system followed **PCI-DSS compliance standards**, meaning we never stored raw card data — everything was handled through **secure tokens and encryption**.

For scalability and reliability, we used **Celery with Redis** for background transaction processing and **PostgreSQL** for transactional data storage.

So overall, the Tap-to-Pay project was about building a **secure, high-performance digital payment system** that allowed users to make **contactless transactions** directly from their mobile banking app.

## Q3. What did you understand by this job role? and how you fit for this role?

Ans: This role focuses on developing secure, scalable backend systems for mobile payment applications — similar to Tap-to-Pay or Apple Pay — using Python. It involves building APIs for digital wallet integration, card tokenization, and real-time transaction authorization, while ensuring PCI-DSS compliance and data encryption.

I’m a strong fit for this position because I’ve worked on a similar **Tap-to-Pay project at Flagstar Bank**, where I developed Python-based backend services for digital wallet and card tokenization. I built secure RESTful APIs to communicate with card networks for transaction authorization and implemented token-based encryption to ensure PCI compliance. With over **5 years of hands-on Python experience** in **financial systems, API development, and payment security**, I have a solid background that aligns perfectly with the requirements of this role.

