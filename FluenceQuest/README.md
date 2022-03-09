# Fluence Quest System

A mockup idea for a gamified system of quests that awards users for their learning. 
The basic idea is a game system using NFT's that keep track of the user's progress and change appearance and perks as the user progresses in the quest system. This system would use the compute protocol as well as blockchain technology to validate and decentralize the progress of each player.

## Fluence Badge Case

This would be a non-transferrable ERC-721 that would be used as a decentralized ID by the players.
This would be minted by the players when registering to the game and it would only allow one per address.
The NFT would have the following attributes:

- Rank:
This would be the member's current rank. This would be calculated using Fluence's decentralized backend.
- Badges:
This would be a list of badges that would be displayed in it.
- Owner:
The address or ENS domain of the holder.
- Customization Metadata:
Any other customization for the dynamic NFT such as colors, styling, and other unlockables.

The presentation of the NFT would be an HTML file that takes parameters in the URL. 
Most NFT marketplaces nowadays support HTML views for NFT's, so this could be used to have fully on-chain metadata and having the NFT's smart contract just appending the parameters to the token URI.

i.e. `www.example.org/token?color=black&rank=4`

## Fluence Quest System

The game itself would be a system of quests that show practical uses of fluence's backend.
The documentation can be a bit overwhelming for newcomers and a multiple choice quiz isn't the way to learn about the technology. 
Instead, the quest system should have bite-sized lessons that show the basics of how things work and then gradually show them how to do things themselves. 
This would make the lessons easy to follow and gradually more challenging.
The practical lessons could have a embedded IDE on the website side by side with the content. 
For example, a tutorial with how to build a helloworld should show the IDE side by side with the .rs file and ask the user to change the message, with the next step explaining what each part does. 

The lessons would then be organized and grouped by chapters. The completion of each chapter would then increase the rank of each user and validating it using the decentralized backend. 


## Curriculum

The course curriculum should be designed to go through all the basics and then gradually add more practical lessons that slowly do less hand-holding. 
A sample curriculum could be:

- Learning Path 1: Basics of Aquamarine
	- Basic concepts
	- Particles/Aqua/Marine explanations with interactive flowcharts.
- Learning Path 2: Aqua Language 
	- Hello world
	- Typing basics
	- Execution flow
	- Basic programs
- Learning Path: Services
	- Architecture of hosted services and browser to services
	- Building a service
- Learning Path: Oracles
	- Basics of oracles
	- Building an oracle

## Quest Completion

Curriculums could be linear or parallel, allowing different learning paths to be completed.
Each lesson should have the backend validate that the user completed each exercise correctly in the IDE. 
As the user completes chapters in a learning path, the backend should update the information of the NFT and the badge should start partially taking shape. 
Once all chapters in a path are completed, the badge could take its full shape and display a glowing effect.


## Verification

After all the learning path's chapters have been completed and the user has obtained all the badges, it could also be possible to have the user build a small project and have members of the fluence team look at it and "verify" their badges by adding community roles off-chain. This could give the community a list of "verified developers." 
