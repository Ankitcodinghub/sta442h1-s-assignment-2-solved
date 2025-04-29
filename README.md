# sta442h1-s-assignment-2-solved
**TO GET THIS SOLUTION VISIT:** [STA442H1 S Assignment 2 Solved](https://www.ankitcodinghub.com/product/sta442h1-s-assignment-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117155&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;STA442H1 S Assignment 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
1. For this question you have to simulate a dataset. Let’s assume the outcome Y depends on 50 covariates X1,X2,…,X50 linearly. That is the relationship is presented with the following equation:

Y = β0+ β1X1+ β2X2+ ··· + β50X50+ ϵ (1)

• Generating training sets of size 100. That is,

– Generate 100 random values of all X variables from standard normal distribution.

That is X1 ∼ N(0,1),X2 ∼ N(0,1)…X50 ∼ N(0,1)

– Generate ϵ also from standard normal ϵ ∼ N(0,1)

– Generate βs from some Uniform distribution where β1 to β20 are simulated from Uniform(0.5, 1.5) and β21 to β50 are simulated from Uniform(0.2, 0.4)

– Then generate Y using (1)

• Generating test set of size 1000,

– Generate 1000 random values of all X variables from standard normal distribution. That is X1 ∼ N(0,1),X2 ∼ N(0,1)…X50 ∼ N(0,1)

– Generate ϵ also from standard normal ϵ ∼ N(0,1) – Use the same βs generated for the training set.

– Then generate Y using (1)

1

2. For this problem you need to load the NHANES dataset using the following command

## If the package is not installed then use ##

install.packages(‘NHANES’) ## And install.packages(‘tidyverse’) library(tidyverse) library(NHANES) small.nhanes &lt;- na.omit(NHANES[NHANES$SurveyYr==”2011_12″

&amp; NHANES$Age &gt; 17,c(1,3,4,8:11,13,25,61)]) small.nhanes &lt;- small.nhanes %&gt;% group_by(ID) %&gt;% filter(row_number()==1)

This is data collected by US National Center for Health Statistics (NCHS). The preceeding codes creates a small dataset of the original NHANES dataset. With this dataset answer the following questions,

small.nhanes &lt;- na.omit(NHANES[NHANES$SurveyYr==”2011_12″ &amp; NHANES$Age &gt; 17,c(1,3,4,8:11,13,25,61)])

Fit a mixed effects logistic regression. Only consider random intercept for subject ID. Use all the available predictors. Interpret the results.

2
