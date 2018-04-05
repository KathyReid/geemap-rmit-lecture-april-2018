# GEEmap - mapping Geelong's entrepreneurial ecosystem

## Introduction

Slide: Introduction

Thanks PRESENTER.

I'm Kathy Reid, and I work as an independent technology consultant in Geelong. As you might be aware, Geelong is undergoing a period of rapid transformation - many of the large manufacturing industries in Geelong are closing and so the economy is being forced to transform to as service and knowledge based economy - and entrepreneurialism is a big part of that - in fact it's a key part of the City's 'Clever and Creative' 30 year strategic plan.

Many of the actors in Geelong:

* Enterprise Geelong - the City's economic development unit
* Entrepreneurs Geelong
* Skilling the Bay
* Deakin University Manufutures

have recognised this problem and have come together to develop GEEmap.

## Problem

SLIDE: What's the problem

So, what problem are we trying to solve?

We want to know

* what the ecosystem looks like
* where the gaps are
* where there are overlaps

and in turn this will help us to

* drive development of the ecosystem

## Approach

SLIDE: What's the approach?

The project approach to GEEmap was in several stages

* Literature review
* Survey
* Analysis and results to drive development
* Data visualisation


## Literature review

SLIDE: Literature review

The literature review looked at all the empirical research on entrepreneurial ecosystems. This is a really new field for research, and there weren't very many papers - only around 20 or so. We synthesized the findings from these papers into nine key *pillars* - listed here.

There is no universally accepted taxonomy of entrepreneurial ecosystems, and our pillar definition is a step in this direction.

We then defined criteria that organisations would need to meet to be associated with each pillar - we probably don't have enough time today to go into those in detail - but unsurprisingly, many organisations wanted to be associated with multiple pillars.

## Survey

SLIDE: Survey

A survey was administered, and among other findings - which you can see on the GEEmap website, this provided the information required to identify organisations and associate them with pillars.

The survey also highlighted several gaps and overlaps in the ecosystem - such as a lack of angel funding and investment capital, and significant overlaps in networking communities and support services

## Mapping nodes

The survey data allowed us to map the nodes - organisations and pillars - and the links between them.

This was done in JSON as the data format is easy to manipulate in the d3.js library, and is also easy to replicate when outputting data from a database to a flat file format.

## Alternatives for data visualisation

Once we had the node and link mappings, we were then able to explore different ways of visulaising the data.

### Packed circles

The packed circles visualisation gave us a good idea of how big each pillar of the ecosystem was, and how many organisations there were in the pillar. However, it didn't show links between nodes, and even with the survey data, we didn't have an effective or community-appropriate way of identifying the *size* of organisations - for instance many organisations wouldn't have been comfortable telling us their annual turnover.

### Concentric circles

Like a solar system map, this tried to show the denisty of organisations in comparison to each other. Again, this was rejected because the links were not visualised.

### Clustered circles

The clustered circles looked great, but again the links between organisations were not visualised

### Sticky force directed

We then started to explore using sticky force directed graphs, and these seemed more appropriate. It took several iterations though before we got a result that was both visually attractive and conveyed the links and connections in the way that we wanted.

### Final visualisation

And this is the version we settled on.

You can see that we haven't differentiated the size of organisations - because we couldn't find an effective metric to do this on.

#### Interactive

We can see the interactive visualisation here

And there's some neat tricks - when you mouse over a pillar, all the organisations change colour, and you can 'pin' an organisation or pillar in place to help you better explore the ecosystem.

Mousing over provides the details of the organisation

## Challenges

* Size of organisations
* Graph force
* Text wrapping
* Interactivity and mouse over areas


## Future directions

* Change over time
* Visualisation hierarchy
* Organisation attributes


## Questions and thank you
