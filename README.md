# Credit-Risk-Modeling

# Credit Risk Key Metrics

## 1️⃣ PD – Probability of Default

**Definition:**

* The probability that a borrower will default within a specific time period.

**Formula:**

```
PD = (Number of Defaults) / (Total Number of Loans)
```

**Example:**

* 1000 loans, 30 defaults:

```
PD = 30 / 1000 = 0.03
```

---

## 2️⃣ LGD – Loss Given Default

**Definition:**

* The proportion of the exposure that is lost if a default occurs.
* Usually calculated as 1 minus the recovery rate.

**Formula:**

```
LGD = 1 - (Recovery Amount / Exposure at Default)
```

**Example:**

* Loan amount = 100,000, recovered = 30,000:

```
LGD = 1 - (30,000 / 100,000) = 0.7
```

---

## 3️⃣ EAD – Exposure at Default

**Definition:**

* The total value the bank is exposed to at the time of default.
* Includes outstanding balance + utilized portion of unused credit lines.

**Formula:**

```
EAD = Outstanding Balance + Utilized Portion of Unused Credit Lines
```

**Example:**

* Balance = 80,000, unused limit = 20,000:

```
EAD = 80,000 + 20,000 = 100,000
```

---

## 4️⃣ EL – Expected Loss

**Definition:**

* The expected monetary loss on a loan or portfolio, combining PD, LGD, and EAD.

**Formula:**

```
EL = PD * LGD * EAD
```

**Example:**

* PD = 0.03, LGD = 0.7, EAD = 100,000:

```
EL = 0.03 * 0.7 * 100,000 = 2,100
```
