# 5th
#customer details
class Customer  
@@total_customers = 0  
def initialize(name, age, email)  
@name = name  
@age = age  
@email = email  
@@total_customers += 1  
end  
def display_details  
puts "Customer details:"  
puts "Name: #{@name}"  
puts "Age: #{@age}"  
puts "Email: #{@email}"  
end  
def self.total_number_of_customers  
puts "Total number of customers: #{@@total_customers}"  
end  
end  
# Creating customer objects  
cust1 = Customer.new("pradeep ", 21, "praeep@example.com")  
cust2 = Customer.new("shivaji", 20, "shivaji@example.com")  
# Displaying customer details  
cust1.display_details  
puts "\n"  
cust2.display_details  
puts "\n"  
# Displaying total number of customers  
Customer.total_number_of_customers 
