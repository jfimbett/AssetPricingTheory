# Asset Pricing Theory - Ph.D. Course

Advanced Ph.D. level course on Asset Pricing Theory taught at the M104 Master of Research in Finance at Paris Dauphine-PSL.

## Course Information

- **Instructor**: Juan F. Imbet
- **Email**: juan.imbet@dauphine.psl.eu
- **Position**: Assistant Professor of Finance
- **Institution**: Paris Dauphine University-PSL
- **Duration**: 10 sessions of 3 hours each
- **Prerequisites**: Foundation courses on Microeconomics

## Learning Objectives

To understand and apply key theoretical models in asset pricing to be able to develop original models and to prepare students for Empirical Asset Pricing.

## Grading Structure

- 70% Final exam
- 30% Two homework assignments

## Course Structure

This repository contains all course materials organized by day:

### Day 0: Course Introduction
- **Syllabus**: Presentation of the course.

### Day 1: Fundamentals of Asset Pricing
- **Syllabus**: Begin with the law of one price and the stochastic discount factor (SDF). Develop the Arrow–Debreu state-space framework and the fundamental theorem of asset pricing. Discuss arbitrage, market completeness and the relationship between state prices and risk-neutral probabilities. Introduce the pricing kernel and show how it prices simple assets and derivative securities. Motivate consumption-based asset pricing as a unifying principle.
- **Key Topics**: law of one price; SDF and state price density; arbitrage and fundamental theorem; complete vs incomplete markets; Arrow–Debreu equilibrium; risk-neutral measure; derivative pricing basics.
- **Practical Focus**: derive state prices in a one-period model; compute pricing kernels for discrete economies; construct replicating portfolios in a stylized model.

### Day 2: Portfolio Choice and Static Asset-Pricing Models
- **Syllabus**: Develop investor preferences and optimal consumption–portfolio choice. Cover mean-variance analysis, HARA utility and two-fund separation. Introduce the Capital Asset Pricing Model (CAPM) and the Arbitrage Pricing Theory (APT) as static equilibrium models. Discuss factor structures in equilibrium.
- **Key Topics**: expected utility; efficient frontier and mean–variance analysis; HARA and Cass-Stiglitz two-fund separation; CAPM and consumption-based CAPM; APT.
- **Practical Focus**: solve optimal portfolio problems under quadratic and CRRA utility; demonstrate two-fund separation; derive CAPM from equilibrium.

### Day 3: Dynamic Asset Pricing and Intertemporal Models
- **Syllabus**: Introduce dynamic programming and continuous-time methods for portfolio choice. Derive Merton's consumption–investment problem and the intertemporal CAPM. Extend the consumption-based model to habit formation and recursive preferences. Explain state-variable dynamics, market incompleteness and dynamic equilibrium.
- **Key Topics**: dynamic programming; Merton model; intertemporal CAPM; CCAPM; habit formation; recursive preferences; continuous vs discrete-time modeling.
- **Practical Focus**: solve Merton's model analytically; set up Euler equations for the CCAPM; analyze comparative statics under different preference specifications.

### Day 4: Fixed-Income and Derivative Pricing
- **Syllabus**: Cover risk-neutral pricing for bonds and derivatives. Introduce the term-structure models (Vasicek, Cox–Ingersoll–Ross, affine models). Discuss option pricing (binomial trees, Black–Scholes) and how derivative prices reveal the SDF. Introduce continuous-time asset pricing and stochastic calculus.
- **Key Topics**: risk-neutral measure; Vasicek and CIR models; Heath–Jarrow–Morton framework; option pricing; affine term-structure models.
- **Practical Focus**: derive closed-form bond prices in Vasicek and CIR; compute option values with binomial trees; show how option prices restrict the SDF.

### Day 5: Market Frictions, Transaction Costs and Incomplete Markets
- **Syllabus**: Examine how frictions alter asset pricing. Topics include transaction costs, borrowing constraints, liquidity shocks and incomplete markets. Discuss models with habit formation and recursive utility under frictions. Introduce production-based models where investment frictions affect asset prices.
- **Key Topics**: transaction costs; segmented markets; borrowing constraints; limited participation; production-based asset pricing; market incompleteness.
- **Practical Focus**: build stylized models with proportional transaction costs; analyze equilibrium under borrowing constraints; illustrate production-based pricing with a simple neoclassical firm.

### Day 6: Information, Asymmetric Information and Market Microstructure
- **Syllabus**: Study how information is incorporated into prices. Grossman–Stiglitz model and rational expectations equilibrium. The no-trade theorem, Kyle's insider-trading model, and Glosten–Milgrom sequential trade model. Discuss noise traders, order books and liquidity provision. Theoretical links between information and asset prices.
- **Key Topics**: asymmetric information; rational expectations; no-trade theorem; Kyle and Glosten–Milgrom models; liquidity and price impact; information diffusion.
- **Practical Focus**: derive equilibrium pricing in Kyle's model; work through the Glosten–Milgrom sequential trade game; analyze comparative statics of information precision.

### Day 7: Intertemporal Risk and Long-Horizon Models
- **Syllabus**: Explore long-run risk, rare disasters and models with Epstein–Zin preferences. Analyze how time-varying investment opportunities and state variables affect equilibrium pricing. Discuss recursive utility and separation of risk aversion from intertemporal substitution.
- **Key Topics**: long-run risk; rare disaster models; Epstein–Zin utility; stochastic volatility in consumption; implications for risk premia.
- **Practical Focus**: derive asset-pricing implications of Epstein–Zin preferences; solve rare disaster model equilibria; illustrate comparative statics with long-run risk.

### Day 8: Macro-Finance, Intermediary Asset Pricing and Production-Based Models
- **Syllabus**: Connect asset prices with macroeconomics and corporate finance. Cover intermediary-based models where financial institutions act as marginal investors. Examine production-based asset pricing with investment frictions, risk shocks and search frictions. Integrate human and labor capital into pricing kernels.
- **Key Topics**: intermediary asset pricing; leverage-based risk premia; production-based models; human capital; macro-finance links.
- **Practical Focus**: derive equilibrium with constrained intermediaries; show how leverage enters the SDF; model investment-specific technology shocks.

### Day 9: Behavioral and Household Finance (Theoretical Foundations)
- **Syllabus**: Introduce behavioral deviations from rational expectations. Prospect theory, ambiguity aversion, non-exponential discounting, and limits to arbitrage. Theoretical household finance: life-cycle portfolio choice, housing and illiquid assets, borrowing constraints and heterogeneity.
- **Key Topics**: prospect theory; ambiguity; noise trader risk; limits to arbitrage; life-cycle models; portfolio choice with illiquid assets; heterogeneity in preferences.
- **Practical Focus**: set up prospect-theory utility maximization; solve a stylized life-cycle consumption–savings model; analyze equilibrium implications of behavioral preferences.

## Repository Structure

```
├── index.html                 # Main course landing page
├── README.md                  # This file
├── LICENSE                    # MIT License
├── TODO.md                    # Development checklist
├── src/                       # Source files and templates
│   ├── styles.css            # CSS styling for all course materials
│   └── DAY_TEMPLATE.md       # Template for creating new days
├── images/                    # Course assets and branding
├── preliminaries/             # Prerequisites and setup materials
├── day0/                      # Course introduction
├── day1/                      # Fundamentals of Asset Pricing
├── day2/                      # Portfolio Choice and Static Models
├── day3/                      # Dynamic Asset Pricing
├── day4/                      # Fixed-Income and Derivatives
├── day5/                      # Market Frictions
├── day6/                      # Information and Microstructure
├── day7/                      # Intertemporal Risk
├── day8/                      # Macro-Finance
└── day9/                      # Behavioral and Household Finance
```

Each day contains:
- `lecture/` - Quarto-based slides and theoretical materials

## Technical Requirements

### Software Dependencies
- [Quarto](https://quarto.org/) for rendering slides and documentation
- LaTeX for mathematical notation (included with Quarto)

### Setup Instructions

1. **Install Quarto**:
   - Download from [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)
   - Follow installation instructions for your operating system

2. **Render Course Materials**:
   ```bash
   quarto render
   ```

## Usage

### For Students
- Start with the `preliminaries/` folder to review prerequisites
- Navigate through days sequentially using the main landing page
- Review lecture slides and theoretical materials

### For Instructors
- Modify content in `.qmd` files and re-render with Quarto
- Add additional theoretical content or examples as needed

## Contributing

This course is under active development. Please see `TODO.md` for current development priorities.

## License

This work is licensed under the MIT License. See `LICENSE` file for details.

## Contact

**Juan F. Imbet**  
Assistant Professor of Finance  
Paris Dauphine University-PSL  
Email: juan.imbet@dauphine.psl.eu

---

*Last updated: September 2025*
