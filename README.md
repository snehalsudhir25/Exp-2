# Experiment 2: Data Visualization Using Matplotlib and Seaborn

## Aim

To visualize data using Matplotlib and Seaborn libraries.

## Algorithm
1.  **Start.**
2.  Import the Matplotlib and Seaborn libraries.
3.  Load data into a Pandas DataFrame.
4.  Plot a histogram for age distribution using `plt.hist()`.
5.  Plot a scatter plot for Age vs. Salary using `sns.scatterplot()`.
6.  Plot salary distribution using `sns.boxplot()`.
7.  Show the plots sequentially.
8.  **Stop.**


## Program
    import pandas as pd
    import matplotlib.pyplot as plt
    import seaborn as sns
    
    # Create dataset
    data = {
        'Name': ['Arun', 'Kumar', 'Ravi', 'Suresh', 'Ajay',
                 'Vijay', 'Praveen', 'Manoj'],
        'Age': [22, 25, 28, 30, 35, 40, 32, 27],
        'Salary': [20000, 25000, 30000, 35000,
                   45000, 50000, 40000, 28000]
    }
    
    # Create DataFrame
    df = pd.DataFrame(data)
    
    # Display dataset
    print(df)
    
    # 1. Histogram
    plt.figure(figsize=(6, 4))
    plt.hist(df['Age'], bins=5, edgecolor='black')
    plt.title('Age Distribution')
    plt.xlabel('Age')
    plt.ylabel('Frequency')
    plt.show()
    
    # 2. Scatter Plot
    plt.figure(figsize=(6, 4))
    sns.scatterplot(x='Age', y='Salary', data=df)
    plt.title('Age vs Salary')
    plt.xlabel('Age')
    plt.ylabel('Salary')
    plt.show()
    
    # 3. Box Plot
    plt.figure(figsize=(6, 4))
    sns.boxplot(y='Salary', data=df)
    plt.title('Salary Distribution')
    plt.ylabel('Salary')
    plt.show()

 ## output
          Name  Age  Salary
    0     Arun   22   20000
    1    Kumar   25   25000
    2     Ravi   28   30000
    3   Suresh   30   35000
    4     Ajay   35   45000
    5    Vijay   40   50000
    6  Praveen   32   40000
    7    Manoj   27   28000
    Histogram Output
<img width="690" height="440" alt="image" src="https://github.com/user-attachments/assets/3a02f5f2-8c96-4014-be60-01f766d3d7d8" />

    Scatter Plot Output
    
 <img width="689" height="440" alt="image" src="https://github.com/user-attachments/assets/43c768c9-0abd-44a3-8783-19e038ed78cb" />
 
     Box Plot Output
    
 <img width="690" height="440" alt="image" src="https://github.com/user-attachments/assets/cf20fd16-36c6-4539-8f61-fe3f76c980a5" />

## result
The three visualizations were successfully generated using Matplotlib and Seaborn libraries in Python.
