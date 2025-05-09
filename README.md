# FC Barcelona - Super Sub Recommender 🚀

## What's This All About?

Ever yelled at the TV wondering why *that* player is coming on as a sub? Or maybe you've got a hunch about who Barça's real game-changers are from the bench? This project tries to answer those questions with data!

We've built a **"Super Sub Recommender"** that analyzes FC Barcelona player statistics to:

1.  Identify players who make the most significant impact when they come on as substitutes.
2.  Calculate a unique **"Super Sub Impact Score"** to rank these players.
3.  Even simulate match scenarios to suggest who might be the best sub for a given situation!

It's a fun dive into football analytics, trying to quantify that "spark" a substitute can bring.

## What's Inside?

*   **Data Crunching:** We take player season stats, detailed goal logs, and match results.
*   **Smart Stats:** We don't just count goals; we look at things like goals scored *per 90 minutes as a sub*, how a player's presence changes the team's expected goals (`Subs_xG±`), and their overall finishing skill.
*   **The "Super Sub Impact Score"**: Our special formula that combines several key performance indicators into a single score to rank subs.
*   **Cool Visuals:**
    *   Bar charts showing the top-ranked super subs.
    *   Stacked bar charts breaking down *why* top players have high scores.
    *   A heatmap to see how different stats relate to each other and the final score.
    *   A special look at players like Ferran Torres, with charts showing their strengths as a sub.
*   **Match Day Simulator:** A function that takes a hypothetical match situation (e.g., "70th minute, losing 0-1, need a goal!") and recommends top substitute choices.

## Tech Stack

*   **Python 3.x**
*   **Pandas:** For all the data manipulation.
*   **NumPy:** For some number crunching.
*   **Scikit-learn:** For `MinMaxScaler` to get features on the same scale.
*   **Matplotlib & Seaborn:** For making those eye-catching charts!
*   **Deepnote Notebook:** 

## How to Run It Yourself

1.  **Get the Code & Data:** Make sure you have this Jupyter Notebook and the three CSV files:
    *   `results_from_firecrawl_1_barca_subs_dataset.csv`
    *   `results_goal_logs.csv`
    *   `firecrawl_playground_results_matches.csv`
    ...all in the same folder.

2.  **Install the Goodies:** If you don't have them already, install the Python libraries:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn jupyter
    ```

3.  **Fire up Jupyter:** Open your terminal or command prompt, navigate to the folder, and type:
    ```bash
    jupyter notebook
    ```
    Then open the notebook file (it'll probably end in `.ipynb`).

4.  **Run the Cells:** Execute each code cell in order, from top to bottom. Watch the analysis unfold!

## Just So You Know...

*   The "weights" we used for the Super Sub Impact Score are a bit subjective – different opinions could lead to different rankings!
*   The data gives us a lot, but not *everything* (like the exact mood of the player before they ran on).
*   This is mostly focused on attacking impact right now.

Have fun exploring Barça's bench power!
