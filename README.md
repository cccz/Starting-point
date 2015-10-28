# Starting-point

import java.lang.Override;

import com.qualcomm.robotcore.eventloop.opmode.OpMode;
import com.qualcomm.robotcore.hardware.DcMotor;

public class StartingToCentral extends OpMode {
    DcMotor motorFrontLeft;
    DcMotor motorFrontRight;
    DcMotor motorBackLeft;
    DcMotor motorBackRight;
    @Override
    public void init() {
        motorFrontLeft = hardwareMap.dcMotor.get("motor_1");
        motorFrontRight = hardwareMap.dcMotor.get("motor_2");
        motorBackLeft = hardwareMap.dcMotor.get("motor_3");
        motorBackRight = hardwareMap.dcMotor.get("motor_4");
        final static double TREAD_MOTOR_PWR =0.5;

    }
    @Override
    public void start(){
        motorFrontLeft.setPower(TREAD MOTOR PWR);
        motorFrontRight.setPower(TREAD MOTOR PWR);
        motorBackLeft.setPower(TREAD MOTOR PWR);
        motorBackRight.setPower(TREAD MOTOR PWR);
        Thread.sleep(2000);
        motorFrontLeft.setPower(0.0);
        motorFrontRight.setPower(0.0);
        motorBackLeft.setPower(0.0);
        motorBackRight.setPower(0.0);
        motorFrontLeft.setPower(-TREAD MOTOR PWR);
        motorFrontRight.setPower(TREAD MOTOR PWR);
        motorBackLeft.setPower(-TREAD MOTOR PWR);
        motorBackRight.setPower(TREAD MOTOR PWR);
        Thread.sleep(2000);
        motorFrontLeft.setPower(0.0);
        motorFrontRight.setPower(0.0);
        motorBackLeft.setPower(0.0);
        motorBackRight.setPower(0.0);
    }


}
