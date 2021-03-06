Boris Bikes
==================

```
 -------- __@      __@       __@       __@      __~@
 ----- _`\<,_    _`\<,_    _`\<,_     _`\<,_    _`\<,_
 ---- (*)/ (*)  (*)/ (*)  (*)/ (*)  (*)/ (*)  (*)/ (*)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

```
______
 
[Set up](#Setup) | [Interact](#Interact) | [Run Tests](#Tests) | [User Stories](#User-Stories) 

## Afternoon challenge: Boris Bikes
First introduction to pair programming, implementing the follwoing practices:

- Working with user stories
- Domain Modeling
- Feature and Unit testing
- Isolating test with doubles and mocks

Goals:
- Test-drive a simple program using objects and methods
- Pair using the driver-navigator style
- Follow an effective debugging process
- Describe some basic OO principles like encapsulation, SRP

## <a name="Setup">Set up</a>

1. **Fork** this [boris-bike repository](https://github.com/CorinneBosch/boris-bikes/) 
2. Then clone **your** fork to your computer.
3. Ensure you have `Ruby` and `rspec` installed. Check ruby version with `ruby -v`

## <a name="Interact">Interact with the programme</a>

You can frature test and run the boris-bike program in any `code editor` or `IRB`. 

## <a name="Tests">Run tests</a>

To test all units and features at once in your terminal.\
Print out the format documentation with the -fd shortcut.
```
$ rspec
$ rspec -fd
```

To test inividual unit test in your terminal:
```
$ rspec spec/bike_spec.rb -fd
$ rspec spec/docking_station_spec.rb -fd
```

## <a name="User-Stories">The boris-bike challenge is built upon the following user stories:</a>

```
As a person,
So that I can use a bike,
I'd like a docking station to release a bike.

As a person,
So that I can use a good bike,
I'd like to see if a bike is working

As a member of the public
So I can return bikes I've hired
I want to dock my bike at the docking station

As a member of the public
So I can decide whether to use the docking station
I want to see a bike that has been docked

As a member of the public,
So that I am not confused and charged unnecessarily,
I'd like docking stations not to release bikes when there are none available.

As a maintainer of the system,
So that I can control the distribution of bikes,
I'd like docking stations not to accept more bikes than their capacity.

As a system maintainer,
So that I can plan the distribution of bikes,
I want a docking station to have a default capacity of 20 bikes.

As a system maintainer,
So that busy areas can be served more effectively,
I want to be able to specify a larger capacity when necessary.

As a member of the public,
So that I reduce the chance of getting a broken bike in future,
I'd like to report a bike as broken when I return it.

As a maintainer of the system,
So that I can manage broken bikes and not disappoint users,
I'd like docking stations not to release broken bikes.

As a maintainer of the system,
So that I can manage broken bikes and not disappoint users,
I'd like docking stations to accept returning bikes (broken or not).

As a maintainer of the system,
So that I can manage broken bikes and not disappoint users,
I'd like vans to take broken bikes from docking stations and deliver them to garages to be fixed.

As a maintainer of the system,
So that I can manage broken bikes and not disappoint users,
I'd like vans to collect working bikes from garages and distribute them to docking stations.

```

Source of challege requirements: [Makersacadeny - GitHub](https://github.com/makersacademy/course/tree/main/boris_bikes)
