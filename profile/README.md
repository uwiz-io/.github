# uwiz.io

## Who are we
[uwiz.io](https://uwiz.io) is a social platform for traders where they can compete by predicting the future of the markets, to gain score and recognition.

uwiz.io is focused on gamifying trading and investing, allowing users to compete with each other by predicting the future of the markets.


Please check out our cool PWA on mobile here: [uwiz.io](https://uwiz.io)

We also have a Telegram bot with TWA: [@uwiz_bot](https://t.me/uwiz_bot)

## Videos:
[uwiz.io user onboarding UX](https://www.youtube.com/watch?v=QW60nCml0Hg): Shows what a brand new visitor to the platfrom will experience to get familiar with the platform and enroll in the ongloing competition. 

[uwiz.io connecting TON wallet and Proof-of-Prediction smart contract demo](https://www.youtube.com/watch?v=83ShOKLZbrc): 
Shows how the user will be able to connect their TON wallet to their uwiz account. After that they can deploy the [Proof-of-prediction smart contract](https://github.com/uwiz-io/contracts-ton/tree/main/packages/contracts/opinion-verifier) to hash a string repesentation of their predictions and store it on-chain as proof of untampered and timely prediction. Anyone can XOR the sha256 hash of all the verified predictions together and compare the value with the value on the smart contract, if any one of the predictions where tampred with the values would mis-match.

## Repositories guide

### [contracts-ton](https://github.com/uwiz-io/contracts-ton)

This is where we keep the source code for the FunC smart contracts we want to utilize in our platform and their TypeScript interface.

[This is where](https://github.com/uwiz-io/contracts-ton/tree/main/packages/contracts/opinion-verifier) you can see the source code to our Proof-of-Prediction implemantation in FunC. Simply put, this smart contract keeps a 256-bit value that is the result of XORing sha256 of all the strings it has ever gotten by an internal message. By getting a list of all the verified prediction strings, hashing them and XORing them together and comparing the value with the value stored in the smart contract anyone can make sure that none of the predictions where tampered with in any way.

The TypeScript interface and scripts to deploy and send prediction string to this smart contract are also [in this repo](https://github.com/uwiz-io/contracts-ton/tree/main/packages/opinion-verifier).

Here you can also find the standard implementations of Token, NFT, and SBT too.

### [uwiz-ton-react](https://github.com/uwiz-io/uwiz-ton-react)
This is a react UI for interfacing Proof-of-prediction smart contract.

### [backend](https://github.com/uwiz-io/backend)
This is the python backend code of the platform.

### [frontend](https://github.com/uwiz-io/frontend)
This is the vue frontedn code of the platform.

### [telegram-bot](https://github.com/uwiz-io/telegram-bot)
The python source code for [@uwiz_bot](https://t.me/uwiz_bot). Users can submit quick predictions in this bot by sending a Telegram text message (even if they don't have a uwiz acoount yet). They can also open uwiz's TWA.

## About our platform

Users can post their forecasts about various cryptocurrencies and gain or lose points depending on how accurate their predictions turn out to be. The platform also offers rewards and recognition to top performers, which can be a great way to incentivize users to participate.

Additionally, by aggregating the forecasts of the community, uwiz.io can provide a rating for different cryptocurrencies, which can be a valuable resource for investors and traders.

Overall, uwiz.io could be a useful tool for those interested in cryptocurrency trading and investing, as well as a fun way to engage with other like-minded individuals.

Our platform is powered by smart contracts, ensuring that all user logs are transparent and verifiable.

We have ambitious plans. Check out our roadmap: [uwitoken.com/pdf/uwiz_roadmap.pdf](https://uwitoken.com/pdf/uwiz_roadmap.pdf)

We are introducing and working on the concept of Proof of Prediction. Read the paper here: [uwitoken.com/pdf/The_UWI_Token_v0.42.pdf](https://uwitoken.com/pdf/The_UWI_Token_v0.42.pdf)

contacts: hi@uwiz.io • [t.me/khrrt](https://t.me/khrrt) • [t.me/MehsenD](https://t.me/MehsenD) 