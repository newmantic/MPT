# MPT

Modern Portfolio Theory (MPT) is a framework for constructing investment portfolios that aim to maximize expected return for a given level of risk, or equivalently, minimize risk for a given level of expected return. MPT was introduced by Harry Markowitz in 1952 and is foundational in the field of finance.


Expected Return (E[R_p]): The expected return of a portfolio is the weighted average of the expected returns of the individual assets in the portfolio.
E[R_p] = w_1 * E[R_1] + w_2 * E[R_2] + ... + w_n * E[R_n]
Where:
E[R_p] is the expected return of the portfolio.
w_i is the weight of asset i in the portfolio.
E[R_i] is the expected return of asset i.
n is the total number of assets in the portfolio.

Portfolio Variance (Var(R_p)): The variance of the portfolio return is a measure of the total risk of the portfolio. It is calculated based on the variances of individual asset returns and the covariances between them.
Var(R_p) = w_1^2 * Var(R_1) + w_2^2 * Var(R_2) + ... + w_n^2 * Var(R_n) 
          + 2 * (w_1 * w_2 * Cov(R_1, R_2) + w_1 * w_3 * Cov(R_1, R_3) + ... )
Where:
Var(R_p) is the variance of the portfolio return.
Var(R_i) is the variance of the return of asset i.
Cov(R_i, R_j) is the covariance between the returns of asset i and asset j.
w_i and w_j are the weights of assets i and j in the portfolio.

Covariance (Cov(R_i, R_j)): Covariance is a measure of how two assets move together. It is positive if the assets tend to move in the same direction and negative if they move in opposite directions.
Cov(R_i, R_j) = E[(R_i - E[R_i]) * (R_j - E[R_j])]
Where:
E[R_i] is the expected return of asset i.
R_i and R_j are the returns of assets i and j.

Efficient Frontier: The efficient frontier is a set of portfolios that offer the highest expected return for a given level of risk (variance), or equivalently, the lowest risk for a given level of expected return. Portfolios that lie on the efficient frontier are considered "optimal."

Sharpe Ratio: The Sharpe ratio is a measure of risk-adjusted return. It is calculated as the ratio of the portfolio's excess return (over the risk-free rate) to its standard deviation.
Sharpe Ratio = (E[R_p] - R_f) / sigma_p
Where:
E[R_p] is the expected return of the portfolio.
R_f is the risk-free rate.
sigma_p is the standard deviation of the portfolio return (i.e., the square root of Var(R_p)).



Estimate Expected Returns and Covariances:
Calculate the expected return E[R_i] for each asset.
Calculate the covariance matrix Cov(R_i, R_j) for the asset returns.

Construct the Portfolio:
Determine the weights w_i of each asset in the portfolio to minimize the portfolio variance Var(R_p) for a given target return E[R_p].

Optimize the Portfolio:
Use quadratic programming or other optimization techniques to find the portfolio weights that either maximize return for a given level of risk or minimize risk for a given level of return.

Plot the Efficient Frontier:
The efficient frontier is plotted by varying the target return E[R_p] and finding the corresponding minimum variance Var(R_p) for each level of return.
