from fastapi import FastAPI
from fastapi.middleware.cors import CORSMiddleware

# 1. Initialize your FastAPI app
app = FastAPI()

# 2. Add CORS Middleware
# This allows a web application from a different domain to request data from this API.
origins = [
    "*", # Allow all origins for simplicity in this example
]

app.add_middleware(
    CORSMiddleware,
    allow_origins=origins,
    allow_credentials=True,
    allow_methods=["*"],
    allow_headers=["*"],
)

# 3. Define the mind map data structure based on cs1_curriculum.md
mindmap_data = {
    "CS1: Data Science & Statistics Curriculum": {
        "Data Analysis": {
            "Data Analysis Process": {
                "Develop Objectives": {},
                "Identify Data Items": {},
                "Collect Data": {},
                "Process & Format Data": {},
                "Clean Data": {},
                "Conduct Exploratory Analysis": {},
                "Model Data": {},
                "Communicate Results": {},
                "Monitor Process": {}
            },
            "Data Types & Sources": {
                "Primary Data Source": {},
                "Secondary Data Source": {},
                "Cross-sectional Data": {},
                "Longitudinal Data": {},
                "Censored Data": {},
                "Truncated Data": {}
            },
            "Big Data": {
                "Characteristics": {},
                "Volume": {},
                "Velocity": {},
                "Variety": {},
                "Reliability": {}
            },
            "Replication & Reproducibility": {
                "Replication Concept": {},
                "Reproducibility Concept": {},
                "Elements for Reproducibility": {},
                "Value of Reproducibility": {}
            },
            "Descriptive Data Analysis": {},
            "Inferential Data Analysis": {},
            "Moments & Skewness": {
                "Sample Moment": {},
                "Central Sample Moment": {},
                "Coefficient of Skewness": {}
            },
            "Mean, Median, Mode": {
                "Calculation": {},
                "Position for Skewed Distribution": {}
            }
        },
        "Probability Distributions": {
            "Discrete Distributions": {
                "Discrete Uniform": {},
                "Binomial": {},
                "Geometric (Type 1)": {},
                "Geometric (Type 2, Failures)": {},
                "Negative Binomial (Type 1)": {},
                "Negative Binomial (Type 2, Failures)": {},
                "Poisson": {}
            },
            "Continuous Distributions": {
                "Continuous Uniform": {},
                "Normal": {},
                "Lognormal": {},
                "Gamma": {},
                "Exponential": {},
                "Chi-square (χ²)": {},
                "Beta": {},
                "t-distribution": {},
                "F-distribution": {}
            },
            "Joint Distributions": {
                "Joint Probability Function": {},
                "Marginal Probability Function": {},
                "Conditional Probability Function": {},
                "Independence of Random Variables": {},
                "Expected Value of Function of RVs": {}
            },
            "Covariance & Correlation": {
                "Linear Covariance": {},
                "Properties of Covariance": {},
                "Linear Correlation Coefficient": {},
                "Correlation vs Causation": {}
            },
            "Moment & Cumulant Generating Functions": {
                "MGF Definition": {},
                "Moments from MGF": {},
                "CGF Definition": {},
                "Moments from CGF": {},
                "MGF of Sum of RVs": {},
                "MGF of Linear Combination of RVs": {}
            },
            "Poisson Process": {
                "Conditions": {},
                "Time to First Event": {}
            },
            "Simulation": {
                "Inverse Transform Method (Continuous)": {},
                "Inverse Transform Method (Discrete)": {}
            }
        },
        "Sampling & Estimation": {
            "Central Limit Theorem (CLT)": {
                "For Sample Mean": {},
                "For Sum of Sample Values": {},
                "Approximations (Binomial, Poisson, Gamma, Chi-square)": {},
                "Continuity Correction": {}
            },
            "Sample Statistics Distributions": {
                "Sample Mean (Known Variance)": {},
                "Sample Variance (Normal Population)": {},
                "Sample Mean (Unknown Variance)": {},
                "Difference in Sample Means (Known Variances)": {},
                "Difference in Sample Means (Equal Unknown Variances)": {},
                "Ratio of Sample Variances (Normal Populations)": {}
            },
            "Estimators": {
                "Method of Moments (MOM)": {},
                "Maximum Likelihood (MLE)": {},
                "Bias of Estimator": {},
                "Mean Square Error (MSE)": {},
                "Consistency of Estimator": {},
                "Cramér-Rao Lower Bound (CRLB)": {}
            },
            "Confidence Intervals": {
                "Population Mean (Known Variance)": {},
                "Population Mean (Unknown Variance)": {},
                "Population Variance (Normal Population)": {},
                "Binomial Parameter (Large n)": {},
                "Poisson Parameter (Large n)": {},
                "Difference in Means (Known Variances)": {},
                "Difference in Means (Equal Unknown Variances)": {},
                "Ratio of Variances (Normal Populations)": {},
                "Binomial Parameters (Proportions)": {},
                "Poisson Parameters (Means)": {},
                "Prediction Intervals (Known/Unknown Variance)": {},
                "Sample Size Determination": {}
            }
        },
        "Hypothesis Testing": {
            "Core Concepts": {
                "Simple vs Composite Hypothesis": {},
                "Null (H₀) & Alternative (H₁)": {},
                "Type I Error": {},
                "Type II Error": {},
                "Sensitivity": {},
                "Specificity": {},
                "Power of Test": {},
                "P-value": {},
                "Steps of Hypothesis Testing": {}
            },
            "Tests for Single Population": {
                "Mean (Known Variance)": {},
                "Mean (Unknown Variance)": {},
                "Variance (Normal Population)": {},
                "Binomial Parameter (Proportion, Large n)": {},
                "Poisson Parameter (Large n)": {}
            },
            "Tests for Two Populations": {
                "Difference in Means (Known Variances)": {},
                "Difference in Means (Equal Unknown Variances)": {},
                "Equality of Variances (Normal Populations)": {},
                "Equality of Binomial Parameters (Proportions)": {},
                "Equality of Poisson Parameters (Means)": {}
            },
            "Tests for Paired Data": {},
            "Chi-square Tests": {
                "Goodness of Fit": {},
                "Contingency Table (Independence)": {},
                "Reliability of Tests": {}
            },
            "Non-parametric Tests": {
                "Permutation Approach": {},
                "Fisher's Exact Test": {}
            }
        },
        "Correlation & Linear Regression": {
            "Correlation Measures": {
                "Pearson's Sample Correlation Coefficient (r)": {},
                "Spearman's Rank Correlation Coefficient (rs)": {},
                "Kendall's Rank Correlation Coefficient (τ)": {}
            },
            "Correlation Testing": {
                "Test for ρ = 0": {},
                "Test for ρ = ρ₀ (Fisher's Transformation)": {},
                "Spearman's Test for ρs = 0": {}
            },
            "Simple Linear Regression": {
                "Model Definition": {},
                "Response & Explanatory Variables": {},
                "Least Squares Estimates (α̂, β̂)": {},
                "Error Variance (σ̂²)": {},
                "Coefficient of Determination (R²)": {},
                "Confidence Interval for β": {},
                "Confidence Interval for σ²": {},
                "Mean & Individual Response Confidence Intervals": {},
                "ANOVA Table & F-test": {},
                "Residual Analysis": {}
            },
            "Multiple Linear Regression": {
                "Model Definition": {},
                "Parameter Estimation": {},
                "Significance of Parameters": {},
                "ANOVA Table & F-test": {},
                "Model Checking": {},
                "Adjusted R²": {},
                "Variable Selection (Forward/Backward)": {},
                "Interaction Terms": {}
            },
            "Variables & Factors": {
                "Variables (Numerical)": {},
                "Factors (Categorical)": {},
                "Number of Parameters": {},
                "Parameterised Form": {}
            }
        },
        "Generalised Linear Models (GLMs)": {
            "Components": {
                "Distribution of Response Variable (Exponential Family)": {},
                "Linear Predictor (η)": {},
                "Link Function (g(µ))": {}
            },
            "Key Concepts": {
                "Exponential Family Definition": {},
                "Natural Parameter": {},
                "Scale (Dispersion) Parameter": {},
                "Mean, Variance & Variance Function": {},
                "Canonical Link Function": {},
                "Saturated Model": {}
            },
            "Parameter Estimation": {
                "Maximum Likelihood Estimates (MLEs)": {},
                "Fitted Values": {},
                "Significance of Parameters": {}
            },
            "Model Fit & Comparison": {
                "Scaled Deviance": {},
                "Comparing Models (Normal/Non-Normal)": {},
                "Akaike's Information Criterion (AIC)": {},
                "Forward Selection": {},
                "Backward Selection": {}
            },
            "Residuals": {
                "Definition": {},
                "Pearson Residuals": {},
                "Deviance Residuals": {},
                "Checking Model Fit with Residuals": {}
            },
            "Applications": {
                "General Insurance": {},
                "Differences from Multivariate Linear Regression": {}
            }
        },
        "Bayesian Statistics": {
            "Core Concepts": {
                "Bayesian Estimation": {},
                "Prior Distribution": {},
                "Likelihood Function": {},
                "Posterior Distribution": {},
                "Conjugate Prior Distribution": {}
            },
            "Loss Functions & Estimates": {
                "Quadratic Loss": {},
                "Absolute Error Loss": {},
                "All-or-Nothing Loss (Zero-one Loss)": {}
            },
            "Parameter Examples": {
                "Poisson Mean (Gamma Prior)": {},
                "Normal Mean (Normal Prior)": {},
                "Binomial Probability (Beta Prior)": {}
            }
        },
        "Credibility Theory": {
            "Credibility Premium": {
                "Definition": {},
                "Formula": {},
                "Credibility Factor (Z)": {}
            },
            "Models": {
                "Normal/Normal Model": {
                    "Credibility Factor Behaviour": {}
                },
                "Poisson/Gamma Model": {
                    "Credibility Factor Behaviour": {}
                },
                "Binomial/Beta Model": {
                    "Credibility Factor Behaviour": {}
                },
                "Empirical Bayes Credibility Theory (EBCT) Model 1": {
                    "Assumptions": {},
                    "Definitions (m(θ), s²(θ))": {},
                    "Credibility Estimate Formula": {},
                    "Credibility Factor Formula": {},
                    "Similarities with Normal/Normal": {},
                    "Differences from Normal/Normal": {}
                },
                "Empirical Bayes Credibility Theory (EBCT) Model 2": {
                    "Main Difference from EBCT Model 1": {},
                    "Assumptions (Risk Volume)": {},
                    "Credibility Factor Formula (Risk i)": {}
                }
            }
        },
        "R Programming for CS1B": {
            "Data Handling": {
                "Setting/Getting Working Directory": {},
                "Importing Data (RData, txt, csv)": {},
                "Attaching/Detaching Data Frames": {},
                "Entering Data (c())": {},
                "Basic Data Functions (length, sum, mean, median, var, sd, quantile)": {}
            },
            "Mathematical Functions": {
                "factorial(x)": {},
                "choose(n,x)": {},
                "gamma(x)": {},
                "exp(x)": {},
                "log(x)": {},
                "sqrt(x)": {},
                "x^n": {}
            },
            "Logical Tests": {
                "!=": {},
                "==": {},
                ">=": {},
                ">": {},
                "| (or)": {},
                "& (and)": {}
            },
            "Distribution Functions": {
                "dbinom (probability/PDF)": {},
                "pbinom (cumulative probability)": {},
                "qbinom (quantiles)": {},
                "rbinom (random values)": {},
                "Supported Distributions (binom, pois, geom, hyper, nbinom, norm, t, f, exp, gamma, lnorm, chisq, unif, beta)": {}
            },
            "Tables & Graphs": {
                "Frequency Table (table())": {},
                "Bar Chart (barplot())": {},
                "Histogram (hist())": {},
                "General Plot (plot())": {},
                "Adding Lines (lines())": {},
                "Adding Points (points())": {},
                "Adding Straight Lines (abline())": {},
                "QQ Plots (qqnorm(), qqline(), qqplot())": {}
            },
            "CLT Simulation": {
                "Generating Sums of Samples": {},
                "Generating Means of Samples": {},
                "Calculating Probabilities Empirically": {}
            }
        }
    }
}


# 4. Create your API endpoint
@app.get("/api/mindmap")
def get_mindmap_data():
    """This endpoint returns the entire mind map data structure."""
    return mindmap_data
