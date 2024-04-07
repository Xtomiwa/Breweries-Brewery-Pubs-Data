# Breweries & Brew Pubs Analysis

## Table of Contents

- [Project Overview ](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)

### Project Overview 

This project aims to analyze brewery data to gain insights into the brewery landscape across different states and cities in the United States. Through this analysis, actionable insights will be developed to inform strategic decision-making for stakeholders in the brewery industry, including policymakers, investors, and brewery owners. Ultimately, the goal is to support informed decision-making and facilitate future growth within the brewery sector.

### Data Source 

Breweries Data: The primary dataset used for this analysis is the "Breweries_data.csv", contaning a list of over 7,000 breweries and brewpubs in the USA provided by Datafiniti's Business Database. The dataset includes the category, name, address, city, state, and more for each entry.

This data was sourced from Data.world [Download Here](https://data.world/datafiniti/breweries-brew-pubs-in-the-usa)

### Tools

Python(Jupyter)

### Data Cleaning

In the intital data preparion phase, I performed the following task:
1. Data loading and inspection.
2. Handling missing values.
3. Data Cleaning and Formatting.

### Exploratory Data Analysis

EDA involved exploring the breweries data to answer key questions, such as:

- What is the number of breweries in each state?
![Breweries by State](https://github.com/Xtomiwa/Breweries-Pubs-Data/assets/112486285/22c55809-f1d4-43a9-a52d-88ff2fa67ddd)


- What are the cities with the most brew hubs per person?
- What are the states with the most breweries per person?
- What are the top cities for breweries?
- What are the top states for breweries?
- What industry categories are typically grouped with breweries?

### Data Analysis 

Some Interesting code I worked with

``` Jupyter(Python)
Breweries_by_state = df.groupby('province')['name'].count().reset_index()
Breweries_by_state.columns = ['STATE', 'NUMBER OF BREWERIE']
Breweries_by_state
```

### Results

The analysis results are summarized as follows: 
- The top 5 states with the highest number of breweries in the USA are California (CA) - 2707 breweries, followed by New York (NY) - 846 breweries, Florida (FL) - 838 breweries, Texas (TX) - 829 breweries, and Washington (WA) - 814 breweries. These insights illuminate the distribution of breweries across states, offering valuable context for stakeholders in the brewery industry, including policymakers, investors, and brewery owners. Understanding this landscape facilitates informed decision-making and strategic planning based on geographical brewery distribution. Additionally, it lays the groundwork for further examination of factors influencing brewery location and growth trends nationwide.

- In the analysis of the number of breweries per person, it was observed that cities like San Diego, Portland, and Seattle have a relatively high concentration of brew pubs compared to their population size. San Diego, with 213 breweries and a population of 294, exhibits a particularly notable ratio of breweries to residents. Similarly, Portland and Seattle also demonstrate a significant number of breweries per person, with 206 breweries and 182 breweries respectively. Conversely, cities like Milwaukee, despite having a lower number of breweries, have a comparatively higher ratio of breweries to population, indicating a strong presence of breweries relative to the number of residents. These findings highlight the varying brewery landscapes across different cities, suggesting potential factors such as local demand for craft beer and supportive regulatory environments.

- Our analysis also reveals that despite Portland having more brewpubs than Seattle, there are more residents in Seattle who visit or use the brewpubs. This could be attributed to factors such as cultural preferences, with Seattle potentially having a stronger tradition of craft beer consumption. Additionally, Seattle's brewpubs may offer a wider variety or higher quality of craft beer, and they may be more conveniently located and accessible. Effective marketing and promotion strategies by Seattle's brewpubs, along with the city's tourism and visitor traffic, may also contribute to higher patronage.Conversely, cities with fewer brewpubs but higher resident patronage may benefit from factors such as a strong reputation for quality craft beer, special events or attractions hosted by brewpubs, positive word of mouth and community engagement, and the cultural significance of brewpubs as community hubs. These findings underscore the complex interplay of factors influencing resident patronage at brewpubs in different cities, shedding light on the varying brewery landscapes across urban areas.

- California, New York, Florida, Washington, and Texas are the top 5 states with the most breweries per person. This aids in identifying regions where the brewery industry is particularly robust and where there may be a higher demand for craft beer among residents. Additionally, it provides valuable insights for stakeholders allowing them to tailor their strategies and investments based on the geographical distribution of breweries and the potential market opportunities within these states. Understanding the brewery landscape in these states can also inform decisions related to economic development, tourism promotion, and regulatory frameworks surrounding the craft beer industry.

- The assessment of top states and cities for breweries reveals that California, with San Diego as its leading city, boasts the highest number of breweries overall, followed by New York, Florida, Texas, and Washington. These states are home to major urban centers such as Seattle, Portland, Denver, and Chicago, which also feature prominently among the top cities for breweries. The concentration of breweries in these states and cities suggests thriving craft beer scenes and strong consumer demand for locally brewed beer. Additionally, states like Colorado, Pennsylvania, and Oregon make significant contributions to the brewery landscape, reflecting a nationwide trend of growing interest in craft brewing. Overall, this analysis underscores the dynamic and diverse brewery industry across different regions of the United States, highlighting opportunities for further exploration and investment in the craft beer market.

- The analysis of the number of unique industry categories associated with each brewery reveals valuable insights into the diversity and specialization within the brewery industry. Breweries with a higher number of unique industry categories offer a diverse range of products or services, potentially appealing to a wider audience. Conversely, breweries associated with fewer unique industry categories may be more specialized or focused in their offerings. Additionally, breweries branching out into various categories may indicate efforts to adapt to changing consumer preferences and attract a broader customer base, providing them with a competitive advantage in the market.

### Recommendations
Based on the analysis conducted on the brewery landscape in the USA, I recommened the following actions:

1. Market Segmentation: Segment the brewery market based on geographical distribution and consumer preferences within each region. Tailor marketing strategies and product offerings to meet the unique demands of different demographic segments and geographic areas.

2. Expansion Opportunities: Explore expansion opportunities in states with burgeoning brewery industries, such as California, New York, Florida, Washington, and Texas. Consider establishing new breweries or partnering with existing ones to capitalize on the growing demand for craft beer in these regions.

3. Quality Assurance: Focus on maintaining high-quality standards across all aspects of brewery operations, including brewing processes, product consistency, and customer service. Consistently delivering exceptional experiences can help build brand loyalty and attract repeat customers.

4. Collaborations and Partnerships: Forge strategic collaborations and partnerships with local businesses, tourism agencies, and event organizers to enhance brand visibility and attract new customers. Joint promotional activities, sponsorships, and special events can create unique experiences and foster community engagement.

5. Innovation and Differentiation: Continuously innovate and differentiate your brewery offerings to stand out in a crowded market. Experiment with new beer styles, ingredients, and brewing techniques to appeal to evolving consumer tastes. Embrace sustainability practices and socially responsible initiatives to resonate with environmentally conscious consumers.

### Limitations
I had to remove the menus column because it was empty and was not necessary for my analysis. Removing empty columns can help reduce unnecessary complexity in the dataset, making it easier to work with and interpret the remaining data.
