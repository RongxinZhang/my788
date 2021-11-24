# Corcus Interview Nov 2021

**Deadline**: 2 weeks

## Introduction
Artists are using simple tools to generate new and unique artworks using random seeds. You will create a set of tools to seed randomness, generate artworks and a simple react website to display it.

## Deliverable 1:
Create a programmable random number generator. That takes the following params:
- `min`, `max`: Generate numbers within this range.
- `distribution: This takes two arrays array1: `[0.1, 0.89999, 0.0001]`, array2: `["A", "B", "D"]`. The value of this element determines the probability of an item being selected with this change. In this case, there is a 10% chance of selecting "A" and an 89.999% chance of selecting "B" and a 0.01% chance of selecting "C". `[1, 1, 1]` means that the chances of "A", "B" and "C" are all as likely.
- `unqiue`: Each generated number should be entirely unique from the past. e.g if 1 was generated, we should not get another 1. If `min=0` and `max=99`, we should receive exactly 100 numbers from 0 to 99.

**Language**: Typescript

**Framework**: Free to choose


## Deliverable 2:
Create code that will generate 10K unique images similar to the set shown below. 
![ART1](https://user-images.githubusercontent.com/3782456/143325994-2e31f619-96b3-4986-87f9-83f338918190.png) 
![ART2](https://user-images.githubusercontent.com/3782456/143326766-bf613244-514b-42bb-a2ec-f67fdc468b73.png)
![ART3](https://user-images.githubusercontent.com/3782456/143326774-28db680d-85a6-4696-bbd4-626aa152797d.png) 

The function should take in a `seed` number and outputs a new permutation. The `thickness` of each block, the `color`, and `size` of the frame should be programmable. Each image should then have a **MetaData** file which can be used to "regenerate" the same image. This could be the `seed` number, the `size`, and any other information. 

**Language:** Javascript/Typescript

**Framework:** Must use the random number generator you created above.

## Deliverable 3:
A web gallery that displays these images in interesting ways. There will be 2 pages:
1. Full Gallery: Display all 10K images, consider performance, and how can you optimize for this.
2. Detailed Page: Shows each image in a larger image and the **MetaData**

**Language:** Typescript

**Framework:** ReactJS for frontend (Use typescript .TSX)
