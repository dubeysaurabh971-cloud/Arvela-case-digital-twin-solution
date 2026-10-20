# Arvela-case-digital-twin-solution
Interactive digital twin of a packaging cutover: a weekly supply chain simulation that finds a hidden supplier clash between two plants and tests 5,808 plans to choose the best one.

# Clarin Cutover Twin

An interactive digital twin of a packaging cutover. A weekly supply chain simulation finds a hidden supplier clash between two plants and tests 5,808 plans to choose the best one.

**Live demo:** https://dubeysaurabh971-cloud.github.io/clarin-cutover-twin/

## What it shows

1. **It sees the hidden clash.** Two plants on two different ERPs order the same bottle from one supplier. Each plant's spreadsheet shows enough supply; the connected twin shows Poland running short from week 34.
2. **It tests every plan first.** It simulates 5,808 combinations of switch week, order size, shifts and a second supplier, drops those that break the rules, and ranks the rest by total cost ($75k best plan against $406k for a typical manual plan).
3. **It knows who decides.** Routine actions go to an agent; anything that changes what customers receive, or creates a new contract, goes to a person.

## How to use it

1. Click **"C · week 10"** to load a typical manual plan.
2. Compare *Poland spreadsheet says* with *Connected twin says*.
3. Click **"Run the twin"** to find the best plan.

## The model

A deterministic weekly inventory simulation over 52 weeks (bottle stock, line capacity, DC stock, lost sales), with an exhaustive search over the decisions, business-rule constraints and a total-cost objective. Runs entirely in the browser.

*Practice case: "Arvela Group" is a fictional company and all figures are illustrative.*

Saurabh Dubey · Digital Thread & Digital Twin
