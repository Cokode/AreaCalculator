# AreaCalculator
calculating circle area and also calculating area of a rectangle using method overload 


public class AreaCalculator {

    public static final double INVALID_VALUE_MESSAGE = -1.0;

    public static double area(double radius) {
        if (radius < 0) {
            return INVALID_VALUE_MESSAGE;
        }
        return radius * radius * Math.PI;
    }

    public static double area(double x, double y) {
        if(x < 0 || y < 0) {
            return INVALID_VALUE_MESSAGE;
        }
        return x * y;
    }

    public static void main(String[] args) {
        System.out.println(area(5.0)); // called the first area method.
        System.out.println(area(-5.0, 4.9)); // called the second area method. 

    }
}
