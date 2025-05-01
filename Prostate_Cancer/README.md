# My Prostate Cancer EDA Project

Hey! I’m just a self-learner diving into some really interesting data science stuff on my own, and this is one of my mini-projects. I worked on exploring the prostate cancer dataset from Stamey’s 1989 study. It’s about men who were about to get a radical prostatectomy, and the dataset includes clinical measures that might predict PSA levels.

## About the Data

Here’s what’s in the dataset (some of it sounds a bit technical, but it’s pretty cool):

- **lcavol** – log of cancer volume  
- **lweight** – log of prostate weight  
- **age** – patient’s age  
- **lbph** – log of benign prostatic hyperplasia amount  
- **svi** – seminal vesicle invasion (0 or 1)  
- **lcp** – log of capsular penetration  
- **gleason** – Gleason score (tumor grade)  
- **pgg45** – percent of Gleason score 4 or 5  
- **lpsa** – log of PSA level (this is what I’m trying to predict)

The data was already split into training and test sets, which made life easier.

## How to Run This

If you want to try this yourself:

1. Clone the repo or download the notebook.  
2. Make sure you have Python with pandas, matplotlib, and scipy installed.  
3. Open the Jupyter notebook and run through the cells step-by-step.

## What I Did

I started by just exploring the data - checking out distributions, correlations, and basic stats. Then I ran a simple regression to see which variables actually help predict PSA levels.

Some of the graphs really helped me understand which features matter most.

## What I Found

- My initial regression model had a mean prediction error of about **0.521** on the test data.  
- Just guessing the average PSA value from the training set would’ve given me a much worse error of **1.057** - so the model definitely helps!  
- After I dropped predictors with insignificant $z$-scores (basically the ones that didn’t really contribute), the model got even better - the test error dropped to about **0.45**. This shows that sometimes simpler models with only important features work better.  
- The two strongest predictors were **lcavol** (log cancer volume) and **lweight** (log prostate weight), which makes sense since tumor and prostate size relate closely to PSA levels.

## What’s Next for Me

I’m planning to:

- Try out some more advanced regression methods  
- Experiment with feature selection to make the model simpler and better  
- Use cross-validation to check how stable the results are

If you have any tips or questions, I’m all ears!

## About Me

I’m just learning this stuff on my own because I find it fascinating. This project is part of my journey to get better at data science.

Email: nahid.nm57@gmail.com

## License

MIT License - feel free to use or build on this however you want!

---

Thanks for stopping by!
