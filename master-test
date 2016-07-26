# there are 3 dictionarys. key's are like rows in excel.
# to create an empty list, use []
# fill in the []'s.
lloyd = {
    "name": "Lloyd",
    "homework": [90.0, 97.0, 75.0, 92.0],
    "quizzes": [88.0, 40.0, 94.0],
    "tests": [75.0, 90.0]
}
alice = {
    "name": "Alice",
    "homework": [100.0, 92.0, 98.0, 100.0],
    "quizzes": [82.0, 83.0, 91.0],
    "tests": [89.0, 97.0]
}
tyler = {
    "name": "Tyler",
    "homework": [0.0, 87.0, 75.0, 22.0],
    "quizzes": [0.0, 75.0, 78.0],
    "tests": [100.0, 100.0]
}

# create a list with 3 dicts
students = [lloyd, alice, tyler]


# for """each student in your students list print out that `student`'s data:

for student in students:
    print student["name"]
    print student["homework"]
    print student["quizzes"]
    print student["tests"]

	
	# Add your function below!
def average(numbers):
    total = sum(numbers)
    total = float(sum(numbers))
    return (total / len(numbers))
	
	# homework is 10%, quizzes are 30% and tests are 60%
def get_average(student):
    homework = average(student["homework"])
    quizzes = average(student["quizzes"])
    tests = average(student["tests"])
    return (homework * .10) + (quizzes * .30) + (tests * .60)
	
    # assign letter value to each numeric score
def get_letter_grade(score):
    if score >= 90:
        return "A"
    elif score >= 80:
        return "B"
    elif score >= 70:
        return "C"
    elif score >= 60:
        return "D"
    else:
        return "F"

		# return and print lloyd's score. Fucking lloyd.
print "Lloyd's letter score is " + get_letter_grade(get_average(lloyd))


# get the avg of each student and then calculate the average of those averages
def get_class_average(students):
    results = []
    for student in students:
        results.append(get_average(student))
    return average(results)

print get_class_average([alice]) # print alice only
print get_letter_grade([alice])

students = [alice, lloyd, tyler]
print get_class_average(students)
print get_letter_grade(get_class_average(students))
