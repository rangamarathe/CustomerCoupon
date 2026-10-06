# Will a Customer Accept the Coupon?

This project analyzes survey data from the UCI Machine Learning Repository to identify characteristics associated with drivers accepting mobile coupons. The dataset contains 12,684 driving scenarios involving bar, coffee-house, carry-out, inexpensive-restaurant, and higher-priced-restaurant coupons.

## Jupyter notebook

View the complete analysis, code, charts, and detailed conclusions in [prompt.ipynb](prompt.ipynb).

## Data preparation

- Replaced missing values in the `car` field with `unknown` because nearly the entire column was missing.
- Removed observations missing values in the remaining analysis fields.
- Retained 12,079 observations, or 95.2% of the original dataset.
- Found an overall coupon acceptance rate of 56.9% in the cleaned data.

## Summary of findings

### Bar coupons

- Bar habit is the biggest driver: People who already go to bars regularly are far more likely to accept bar coupons.

- Frequency makes a massive difference:
    - Frequent bar-goers (4+ visits/month): 76.2% accepted
    - Occasional/Non-visitors (3 or fewer visits/month): 37.3% accepted

- Other top-performing groups: Acceptance stays very high (about 69–71%) for bar-goers who are over 25, driving without kids, or working in non-agricultural jobs.

- Takeaway: Prior bar-going behavior is the single strongest indicator of coupon interest. While age and passenger context help refine the picture, but does not conclude on direct effect

### Coffee-house coupons

- Overall Acceptance: Just under half of drivers (49.6%) accepted coffee house coupons.

- Habit is Key: Regular coffee-goers (2+ visits a month) accepted coupons at 65.9%, compared to just 34.0% for non-frequent visitors.

- Timing & Context: Acceptance was significantly higher when drivers: 
    - Had no urgent destination (57.8% vs. 40.1% for those in a hurry).
    - Received the coupon at 10 AM or 2 PM (59.3% vs. 42.5% at other times).
    - Got a 1-day expiration instead of 2 hours (58.1% vs. 42.9%).

- Age Has Less Impact: Younger drivers (under 30) accepted at a slightly higher rate (52.9%) than drivers 30 and older (46.8%).

- Key Takeaway: Target existing coffee drinkers when they are relaxed and traveling around mid-morning or mid-afternoon, giving them a longer window to redeem. (Note: These are strong patterns in survey data, not guaranteed cause-and-effect).

