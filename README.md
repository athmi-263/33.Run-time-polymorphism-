package employee2;
class Employee {
    void work() {
        System.out.println("An employee works");
    }
}

class Manager extends Employee {
    @Override
    void work() {
        System.out.println("Manager supervises the team");
    }
}

class Developer extends Employee {
    @Override
    void work() {
        System.out.println("Developer writes code");
    }
}

class Tester extends Employee {
    @Override
    void work() {
        System.out.println("Tester tests the application");
    }
}

public class Employee2 {
    public static void main(String[] args) {
      
        Employee employee;

        
        employee = new Manager();
        employee.work(); // Outputs: Manager supervises the team

        
        employee = new Developer();
        employee.work(); 

    
        employee = new Tester();
        employee.work(); 
    }
}

OUTPUT
Manager supervises the team
Developer writes code
Tester tests the application
# 33.Run-time-polymorphism-
