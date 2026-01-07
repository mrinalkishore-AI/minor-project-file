import pandas as pd
marks = {
"Name": [
        "Aarav", "Vivaan", "Aditya", "Vihaan", "Arjun",
        "Sai", "Krishna", "Ishaan", "Rohan", "Ananya",
        "Diya", "Priya", "Kavya", "Neha", "Pooja",
        "Sneha", "Aditi", "Isha", "Nisha", "Ritika",
        "Rahul", "Aman", "Suresh", "Ramesh", "Mahesh",
        "Kiran", "Sunil", "Vikram", "Anil", "Deepak",
        "Pankaj", "Nitin", "Sachin", "Vikas", "Ajay",
        "Manoj", "Sanjay", "Ravi", "Ashok", "Gaurav",
        "Shubham", "Prakash", "Harish", "Naresh", "Mukesh",
        "Alok", "Rajesh", "Dinesh", "Yogesh", "Saurabh"
    ],
    "Maths": [
        45, 56, 67, 78, 89, 90, 72, 65, 88, 91,
        54, 60, 73, 84, 95, 69, 77, 82, 86, 58,
        64, 71, 79, 85, 92, 48, 55, 63, 70, 76,
        81, 87, 93, 59, 66, 74, 80, 83, 94, 57,
        61, 68, 75, 78, 88, 90, 96, 52, 62, 73
    ],
    "Science": [
        50, 62, 74, 86, 91, 68, 79, 83, 95, 57,
        64, 71, 88, 92, 76, 84, 69, 77, 81, 90,
        55, 63, 70, 78, 85, 93, 60, 67, 73, 80,
        87, 94, 58, 65, 72, 82, 89, 96, 54, 61,
        66, 75, 83, 88, 91, 97, 59, 69, 74, 86
    ],
    "English": [
        48, 59, 71, 82, 94, 66, 77, 85, 90, 53,
        60, 68, 75, 83, 88, 92, 57, 64, 70, 79,
        86, 95, 54, 61, 69, 76, 84, 91, 56, 63,
        72, 80, 87, 93, 58, 65, 73, 81, 89, 96,
        55, 62, 67, 74, 78, 85, 90, 97, 60, 68
    ],
    "History": [
        52, 63, 74, 85, 91, 68, 79, 87, 93, 56,
        64, 71, 80, 88, 95, 59, 66, 73, 81, 89,
        54, 62, 70, 78, 84, 92, 60, 67, 75, 82,
        90, 96, 58, 65, 72, 83, 86, 94, 55, 61,
        69, 76, 88, 91, 97, 57, 63, 74, 80, 85
    ],
    "Computer": [
        55, 66, 77, 88, 94, 61, 72, 83, 90, 58,
        64, 70, 79, 85, 92, 60, 67, 73, 81, 89,
        54, 62, 68, 75, 84, 91, 56, 63, 71, 78,
        86, 93, 59, 65, 74, 82, 87, 95, 57, 69,
        76, 80, 88, 90, 96, 53, 61, 70, 83, 85
    ]
} 
csv_file="employee_salary_dataset.csv"
df=pd.read_csv(csv_file)
excel_file="output.xlsx"
df.to_excel(excel_file,index=False,engine="openpyxl")
print("csv converted to excel successfully")
print(f"saved as:{excel_file}")
df["Sum"]=df.sum(axis=1,numeric_only=True)
df["Average"]=df.mean(axis=1,numeric_only=True)
df["Max"]=df.max(axis=1,numeric_only=True)
df["Min"]=df.min(axis=1,numeric_only=True)
df["Count"]=df.count(axis=1,numeric_only=True)
df["Sum"]=df.sum(axis=0,numeric_only=True)
df["Sum"]=df.sum(axis=0,numeric_only=True)
df["Sum"]=df.sum(axis=0,numeric_only=True)
df["Sum"]=df.sum(axis=0,numeric_only=True)
df["Sum"]=df.sum(axis=0,numeric_only=True)
