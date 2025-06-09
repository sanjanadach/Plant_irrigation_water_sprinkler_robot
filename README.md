void servo1() { // to control servo 1
  int angle1 = RemoteXY.slider_1 * 0.8+40; // equation for min. and max. angle is 105-180
  myservo1.write(angle1);
}
void servo2() { // to control servo 2
  int angle2 = RemoteXY.slider_1 + 50; // equation for min. and max. angle is 105-180
  myservo2.write(angle2);
}

void ultrasonic() {
  long duration, distance;
  digitalWrite(trigPin, HIGH);
  delayMicroseconds(1000);
  digitalWrite(trigPin, LOW);
  duration = pulseIn(echoPin, HIGH);
  distance = (duration/2)/29.1;
  delay(10);
  if (distance <= 7) {
    RemoteXY.led_blue_b = 255;
    RemoteXY.led_red_r = 0;
  }
  else if (distance > 7) {
    RemoteXY.led_blue_b = 0;
    RemoteXY.led_red_r = 255;  
  }
}
