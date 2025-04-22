## Inspiration
Our inspiration for this project comes from the common frustration of not being able to reach the free shipping threshold when shopping or buying groceries online. Many people either end up paying extra for shipping or adding unnecessary items to their cart just to meet the requirement. We wanted to solve this problem by connecting users who are shopping on the same website, allowing them to combine their orders and share the benefits of free shipping. By fostering a community-driven approach to online shopping, this platform not only helps users save money but also encourages smarter, more efficient purchasing habits. Online businesses also benefit from this platform. By encouraging collaborative purchases, businesses see higher transaction volumes, reduced abandoned carts, and enhanced customer satisfaction. It also helps reduce their logistics and shipping costs. Instead of fulfilling multiple smaller orders with separate packaging, handling, and shipping expenses, they can consolidate purchases into a single shipment.

## What it does
You create an account and can make or view listings for and from other people in your zip code. These listings have a store, location of order, and how much more money an order needs to hit the free shipping quota. You can open a chat with a person, and once decided, the initial lister can upload the order receipt and select which items were theirs, and it will divide up the cost among the two buyers. We will then charge the user who didn't make the purchase their share of the order, and once their reception of items is confirmed through a unique PIN, will deposit that money to the purchasers account. The users can discuss the items and also where to meet to exchange the items through our built in chat.

## How we built it
The technologies we used include:

Next.JS as our frontend + backend framework
Google firebase for our database
Socket.io integration for low latency live chat
Google Sign In integration for account authentication
Capital One Hackathon API for bank account simulation
Challenges we ran into
The Capital One Hackathon API was pretty difficult to understand and work with. The relationships between all the different entities(customers, merchants, accounts, purchases, withdrawals, etc. ) were not only confusing and not intuitive, but also missing features. For example, purchases are not tied to account balances, there is no option to specify the amount in a deposit call, and merchants can't pay out other people.

## Accomplishments that we're proud of
We are proud of all the unique and complex features we were able to implement in such a short period of time, whether that be interactive map capabilities displaying the various potential orders based on zip code, Google Auth integration, incorporation of LLMs to parse invoices/statements, and peer-to-peer real-time chat with message history storage.

## What we learned
This hackathon was our team's first experience working with Next.js, making it an exciting opportunity to explore its core features, such as Server-Side Rendering. For the chat feature, we got our hands dirty with web sockets which allowed us to handle live message updates efficiently. It was definitely a challenging yet rewarding experience after it started working.

## What's next for What's in your Cart?
What's next is to flesh out the rating system, finish up the unique pin confirmation and integrate an API such as Stripe or Paypal so that we can link to actual cards and accounts and have actual payments go through.
