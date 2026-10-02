---
title: "Mapping Germany"
date: 2026-10-02
layout: single
---

# Mapping Germany

I have always thought of maps as something physical that helps us understand where places are and how they relate to each other. However, Wilson’s reading made me reconsider what actually counts as a map. One idea that stood out to me was that mapping can happen before anything is actually drawn or displayed. We can already form an understanding of a place through the locations and experiences we remember. This made me think about my own relationship with Germany. I have spent many of my summers in Germany, mostly in Munich, while my grandfather was there for medical treatment. While he was in the hospital, I spent a lot of time exploring the city with my family. We went to museums and theaters, and I spent a lot of my time going to football games. The more I visited, the more I started to feel like I knew Germany quite well. Looking back, I had already formed my own map of Germany through these experiences, even though I had never thought of it that way.

Working with GeoNames allowed me to move beyond the places I already knew and see patterns across the country that I would not have noticed from my own experiences alone. But I also realized that, just as my own understanding of Germany left out places I had never experienced, a dataset can leave things out too. The map created from the data is not necessarily a complete picture of Germany since what we see depends on what has been recorded, how it has been categorized, and what information is available.

## Map

<div style="width:100%; height:70vh;">
  <iframe
    src="{{ '/assets/Maps/DE_featuremap.html' | relative_url }}"
    width="100%"
    height="100%"
    style="border:0;">
  </iframe>
</div>

When I first downloaded the Germany dataset, I was surprised by how much information it contained. There were 220,225 rows and a lot of feature codes to choose from. I decided to choose museums, theaters, stadiums, and airports because these were some of the places I visited most during my time in Germany. For my fourth feature, I initially chose railway stations, but after filtering the data, I found that there were so many locations that the number of points made the map difficult to read. Since I wanted each feature to be clearly visible, I replaced railway stations with airports.

Before creating the map, I had some predictions about what the distribution of these features might look like. I expected museums, theaters, and stadiums to be concentrated mostly in larger cities such as Munich, Berlin, Hamburg, and Frankfurt, and I imagined that rural areas would have fewer of them. As for airports, I expected them to be more spread out across the country, but I did not expect there to be very many.
After filtering the dataset, I was left with 385 museums, 98 airports, 74 theaters, and 49 stadiums. I was not surprised that museums were the largest group, but I was surprised by the number of airports. I could not imagine Germany having 98 airports. It was much higher than I had expected, especially since I had always thought of airports as the large ones I had traveled through. This made me start questioning the feature codes themselves. What exactly does GeoNames classify as an airport? The same question could be asked about the other features. What counts as a museum, theater, or stadium?

Once I created the map, I was able to see patterns that were much harder to notice when I was only looking at the dataset. Some of the predictions I made were correct, but others were not. I expected Berlin to have a much larger concentration of museums, theaters, and stadiums, but it did not stand out as much as I thought it would. Nuremberg, on the other hand, had a very noticeable concentration of museums. Considering the city’s history, this made sense, but I had not expected the difference to appear that clearly on the map. Museums were also spread across many parts of Germany rather than being concentrated only in large cities.

The other features showed different patterns. Airports were much more spread out across the country than I had expected. Theaters were more concentrated around cities, with fewer points outside these areas. Stadiums were the smallest group, with only 49 locations, and appeared more spread apart on the map.

Looking at the map, I also started to think about what was missing. For instance, I could see that Nuremberg had many museum points and that Berlin had fewer than I expected, but the map did not explain why. The points only showed me that a museum was located there. They did not tell me the size of the museum, what type of museum it was, how many people visited it, or its historical or cultural importance. This was not limited to museums. The airport layer did not tell me whether I was looking at a major international airport or a much smaller one. The stadium layer did not show capacity or what sports were played there, and the theater layer did not show the size of the venue or the kinds of performances it hosted. I could see where these places were, but I did not have enough information to understand the differences between them.

This became important when I started comparing cities. Nuremberg having more museum points does not necessarily mean that museums are more important there than in Berlin. In the same way, a city having more stadium or theater points does not necessarily tell me how important those places are to the city. The map showed me patterns in location and number, but I was missing the information needed to fully explain those patterns. 
This made me think more critically about GeoNames as a database. Kitchin and Lauriault describe how databases and repositories are “not simply a neutral, technical means of assembling and sharing data” but are shaped by the processes involved in producing and organizing that information (Kitchin & Lauriault, 2014). I could see this while doing my own assignment because GeoNames did more than give me locations. The way the information was organized into feature codes affected what I could search for, compare, and eventually show on my map. At the same time, some of the information I wanted when interpreting the map was not available through the categories I was using.

<figure>
  <img src="{{ '/assets/images/Museum-Clusters.jpg' | relative_url }}" alt="Map showing museum locations in Germany">
  <figcaption>Figure 2. Museum locations in Germany, highlighting visible concentrations around Berlin and Nuremberg.</figcaption>
</figure>

The feature codes were useful because they allowed me to organize hundreds of locations, but they also simplified them. All 385 museums became part of one category, just as the 98 airports, 74 theaters, and 49 stadiums were each grouped into their own categories. This made it possible for me to compare their locations, but not necessarily the places themselves. Two airports could be very different in size and purpose but still appear the same. The same could be said of two stadiums or two theaters. The database therefore made certain comparisons very easy, especially number and location, while leaving out some of the details I would need to make other comparisons.

My own decisions also shaped what the final map showed. I originally selected railway stations, but there were so many points that I replaced them with airports. That decision completely changed one of the layers on the map. What I found interesting was that none of this decision-making was visible in the final map. Someone looking at it would only see airports and would have no way of knowing that I had originally chosen railway stations or why I decided to remove them. I also chose only four feature codes out of all the information available. Another person could use the exact same file, choose completely different features, and produce a very different map of Germany. 

Kitchin and Lauriault also explain that “Data do not pre-exist their generation; they do not arise from nowhere” (2014). Thinking about the Germany dataset, I realized it was not simply a collection of information that already existed in this exact form. For a place to become a row in GeoNames, information about it had to be collected and organized in a specific way. Decisions had to be made about its name, coordinates, and feature code. These decisions affect what I am eventually able to find and compare. The categories I worked with were therefore not just labels I happened to find in the file. They were part of how the information about Germany had already been organized before I started working with it.

Looking at where the Germany data came from made this clearer. GeoNames uses information from different sources, including German government agencies, mapping authorities, Deutsche Bahn, and local open-data portals. So even though I downloaded one Germany file, the information in it came from different places. Germany also has a GeoNames ambassador, Lukas Eipert, showing that local knowledge and individual contributors were also involved. Together, these sources, people, and categories make up the data assemblage behind GeoNames. This helped me see that the Germany dataset was not created by one source, but was built by bringing different kinds of information together. 

Overall, this project changed the way I would approach maps. Instead of only looking at the final map, I now pay more attention to the choices that went into creating it. I can see myself using this workflow again for my Political Science capstone, especially if I study migration and the geographic distribution of migrant communities which I am interested in. 


