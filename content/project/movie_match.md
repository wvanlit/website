---
title: "Movie Match"
date: 2020-01-19T17:46:24+01:00
tags: [Python, Machine Learning, Graph Databases, Recommendation Systems]
type: ""
image: ""
abstract: ""
draft: false
---
## Find your ideal movie!
Do you ever have trouble choosing which movie to watch?
I sure do! That's why I created *Movie Match*, which recommends movies to users using a movie that they liked.
<!--more-->
For example, I really like Star Wars. So my input might be "Star Wars: Episode IV - A New Hope". These are the recommendations the system gave me:
* Star Wars: Episode V - The Empire Strikes Back
* Star Wars: Episode VI - Return of the Jedi
* Raiders of the Lost Ark
* Matrix, The
* Terminator 2: Judgment Day
* Forrest Gump
* Pulp Fiction
* Back to the Future
* Silence of the Lambs, The
* Jurassic Park

The first 2 recommendations are other Star Wars films, which aren't that useful to me as I've already seen them of course. The others however show movies that are similar to Star Wars, so those are interesting to me.

## Where can I find it?
Well, it's right here on this very website! You can find it under the Apps tab in the header.

## How does it work?
Currently a list of movie ratings are loaded into [Neo4J](https://neo4j.com/), a graph database. For now the project uses a simple *Collaborative Filtering* algorithm, but in the future I want to implement a *Machine Learning* model to do this instead.

## Roadmap
* Use *Machine Learning* instead of *Collaborative Filtering*
* Increase data in the Dataset
* Create a better looking UI
* Let users create profiles with multiple liked and disliked movies. 
* Fix issues with more obscure movies not having any recommendations
