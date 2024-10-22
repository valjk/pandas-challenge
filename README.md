# pandas-challenge
I leveraged Xpert Learning Assistant when converting Spending Ranges (Per Student) to a string in the "Scores by School Spending" section (line 76) due to repeat TypeError:  '<' not supported between instances of 'int' and 'str'
    
    # Convert Spending Ranges (Per Student) to a string
    school_spending_df["Per Student Budget"] = pd.to_numeric(school_spending_df["Per Student Budget"].astype(str).str.replace('[$,]', '', regex=True), errors='coerce') #Xpert Learning Assitant
