Use the given link below and locate the bank marketing dataset. Data Set Link
Perform the below operations:
a. Is there any association between Job and default?
tbl3 <- table(bank$job,bank$default)
chisq.test(tbl3)
> chisq.test(tbl3)

	Pearson's Chi-squared test

data:  tbl3
X-squared = 60.343, df = 11, p-value = 8.008e-09

# Since the P-value is less than 0.5 there is assosiation between job and default.


b. Is there any significant difference in duration of last call between people having housing loan or not?

cor(bank$previous, as.numeric(bank$loan))
[1] -0.01104349

Since there is no correlation there is no difference.


c. Is there any association between consumer price index and consumer?
No


d. Is the employment variation rate consistent across job types?

No, it is not consistent

e. Is the employment variation rate same across education?

No, it is  not.


f. Which group is more confident?

