# Programming Exercise 1
## Computational Thinking Foundations: Python, VS Code, and GitHub
*Editing README.md on the GitHub web interface for testing.*
*Editing README.md on the local repository using VS Code workspace for testing.*

#### Short Introduction of the Programming Exercise: Its Goals & Objectives

The goal **Programming Exercise** is to introduce the computational workflow which will be utilized for the entire course. It is good practice to establish good habits in:
    1. Reproducible environments;
    2. Version-controlled work; and
    3. Inspecting the data before starting analysis.

By the end of this exercise, I'm expected to be able to:
    1. Configure Python in the VS Code workspace using a virtual environment;
    2. Initialize and manage a GitHub repository, specifically the following:
        - Commit
        - Push
        - Pull
    3. Write basic Python scripts for data inspection; and
    4. Explain my work using the lenses of abstraction, representation, responsibility, and scale.

#### Abstraction: What did you choose to inspect, and why?

For this Programming Exercise, I chose to inspect **coffee shops or cafes** in and nearby UP Diliman. Personally, I believe that *to know a place, you should taste their coffee and their cafe environment*. I have been 'cafe-hopping' since my undergrad, and since it is my first time in UPD, I wanted to map the cafes in the area. I want to cafe-hop in UPD and taste coffee from different places, see how they blend and flavor theirs.

By plotting them and visualizing them, I'll be able to figure out which areas I can visit wherein I can maximize my **time, energy, and resources** and visit multiple ones in one go. It can also help me understand how to go around the area from different points of origin. 

#### Representation: What assumptions are you making about the CSV and coordinates?

While creating the CSV file and retrieving their coordinates, I am making the assumption that **these locations will appear as points**. Each, single point is one cafe, placed in coordinates expressed as *x and y* values. Every point has a unique ID, coordinate pairs, cafe name, and street name. Since this serves as location data, I decided to include the street to support the cafe names. This way, I can easily identify where they are on the map. 

I decided to include only this information and not anything else because it might confuse the data I already have. It is merely for location. Other information, such as price range, operating hours, operating days, and others, can be included in other, more detailed datasets.

#### Responsibility: What should the script check automatically vs what a human should check?

When observing the script or code, it should **automatically check whether the data is valid** and whether it contains missing values. The script can also automatically check whether the **required columns are present** and whether their values are correct and/or accurate. Specifically, the script can check whether the **included coordinates fall within the provided range.**

Additionally, the script can check whether the file name is correct when pulled and whether the data path is accurate and in the correct directory. 

On the other hand, I can check whether the dataset I generated is **properly done**, with correct coordinates, names, and unique IDs. I can check whether the data is in the **correct format** before I input it into the file and ensure that it is the actual data being requested. I can check the map to see if the information is **logical**: the coordinates appear in the same place, with the same cafe name, and on the right street.

#### Scale: What problems might happen if the dataset becomes very large?


Just like how our laptops or desktops **slow down when we try to upload, download, or load something big**, the same thing will happen to this should the data become larger, and it is done with the same machine I have at present. Specifically, if the dataset is bigger than what my machine's RAM can handle, it will slow down and **potentially crash.** One way to resolve this is to use a high-performance computer capable of handling it.

On the other hand, another potential problem arises in visualization. With the current setup for visualization, which is a scatter plot, it might be harder to digest it with potentially thousands or millions of data points involved. Each point will be **clustered together** if it is close to others; leaving no room for proper distinction per point as they would appear like a big, solid block. During the plotting process as well, since there is a lot of data, it could **freeze**. High-performance computers with a capable or appropriate GPU can help with this one.