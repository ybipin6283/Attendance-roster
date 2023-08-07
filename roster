import random

employees = ['Abhishek', 'Siddhesh', 'Ashish', 'Rohit', 'Akshit', 'Siddhant', 'Rijo', 'Warke', 'Omkar_Kamble', 'Vipul', 'Bipin', 'Devendra', 'Madhan', 'Nagendra', 'Ragini', 'Venkatesh']
num_days = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday']
dict = { 'Abhishek': 0, 'Ashish': 0, 'Siddhesh': 0, 'Rohit': 0, 'Akshit': 0,'Siddhant': 0,'Rijo': 0,'Warke': 0,'Omkar_Kamble': 0, 'Vipul': 0,'Bipin': 0,'Devendra': 0,'Madhan': 0,'Nagendra': 0,'Ragini': 0,'Venkatesh': 0}

for day in num_days:
    wed=[]
    for counter_check in dict:
        if dict[counter_check] >= 3:
            if counter_check in employees:
                employees.remove(counter_check)
        elif day == "Tuesday":
            if dict[counter_check] == 0:
                wed.append(counter_check)
        elif day == "Wednesday":
            if dict[counter_check] == 1:
                wed.append(counter_check)
        elif day == "Thursday":
            if dict[counter_check] == 1:
                wed.append(counter_check)
        else:
            wed.append(counter_check)

    if day == "Tuesday" and len(wed) < 9:
        for counter in dict:
            if dict[counter] == 1:   
                if len(wed) < 9:
                    wed.append(counter)
                else:
                    break
    
    if day == "Thursday" and len(wed) < 10:
        for counter in dict:
            if dict[counter] == 2:   
                if len(wed) < 10:
                    wed.append(counter)
                else:
                    break

    if day == "Wednesday":
        daily_list = ((random.sample(wed,11)))
        for nm in daily_list:
            dict[nm] += 1
        print(day + ",")
        print(*daily_list, sep=",")

    elif day == "Thursday":
            daily_list = ((random.sample(wed,10)))
            for nm in daily_list:
                dict[nm] += 1
            print(day + ",")
            print(*daily_list, sep=",")

    else:
            daily_list = ((random.sample(wed,9)))
            for nm in daily_list:
                dict[nm] += 1
            print(day + ",")
            print(*daily_list, sep=",")

print(dict)
