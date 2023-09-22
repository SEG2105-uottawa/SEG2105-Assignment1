package design2;
import java.util.Scanner;

public class PointCP2{

	private double rho;
	private double theta;
	
	public PointCP2(double r, double t) {
		rho = r;
		theta = t;
	}
	
	public double getRho() {
		return rho;
	}
	
	public double getTheta() {
		return theta;
	}
	
	public double getX() {
		return rho * Math.cos(theta);
	}
	
	public double getY() {
		return rho * Math.sin(theta);
	}
	
	public double getDistance(PointCP2 p) {
		return (getX() - p.getX()) * (getX() - p.getX()) + (getY() - p.getY()) * (getY() - p.getY());
	}
	
	public PointCP2 rotatePoint(double d) {
		return new PointCP2(rho, theta + Math.toRadians(d) % (2 * Math.PI));
	}
	
	public String toString() {
		return String.format("Stored as Polar [%f, %f]", rho, theta);
	}
}
