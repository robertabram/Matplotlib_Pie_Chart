# Matplotlib_Pie_Chart


from matplotlib import pyplot as plt

plt.style.use('fivethirtyeight')

slices = [59219, 55466, 47544, 36443, 35917]
labels = ['JavaScript', 'HTML/CSS', 'SQL', 'Python', 'Java']
explode = [0,0,0,0.1,0] # identify space in comparison to radius in percents 

#startangle change the angle of specified part to the right by degrees
#autopct='%1.1f%%' show the measure of every pie in percents
plt.pie(slices,labels=labels,explode=explode,shadow=True,autopct='%1.1f%%',startangle=150,wedgeprops={'edgecolor':'black'})

plt.title('My piechart')
plt.tight_layout()
plt.show()

# Blue = #008fd5
# Red = #fc4f30
# Yellow = #e5ae37
# Green = #6d904f
