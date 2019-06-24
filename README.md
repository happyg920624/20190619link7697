/*
 * Generated using BlocklyDuino:
 *
 * https://github.com/MediaTek-Labs/BlocklyDuino-for-LinkIt
 *
 * Date: Wed, 19 Jun 2019 11:39:49 GMT
 */

#include <LRemote.h>

LRemoteLabel label1;
LRemoteButton button1;
LRemoteCircleButton circle1;
LRemoteSwitch switch1;
LRemoteSlider slider1;

void setup()
{
  LRemote.setName("gracelin2003");
  LRemote.setOrientation(RC_PORTRAIT);
  LRemote.setGrid(5, 6);
    label1.setPos(0, 2);
    label1.setText("Remote Testing");
    label1.setSize(5, 1);
    label1.setColor(RC_GREY);
    LRemote.addControl(label1);

    button1.setPos(2, 1);
    button1.setText("press me");
    button1.setSize(3, 1);
    button1.setColor(RC_ORANGE);
    LRemote.addControl(button1);

    circle1.setPos(3, 3);
    circle1.setSize(3, 1);
    circle1.setText("!big");
    circle1.setColor(RC_ORANGE);
    LRemote.addControl(circle1);

    switch1.setPos(0, 1);
    switch1.setSize(2, 1);
    switch1.setText("USR LED");
    switch1.setColor(RC_ORANGE);
    LRemote.addControl(switch1);

    slider1.setPos(0, 2);
    slider1.setSize(5, 1);
    slider1.setText("value slider");
    slider1.setValueRange(0, 100, 1);
    slider1.setColor(RC_ORANGE);
    LRemote.addControl(slider1);
  LRemote.begin();
}


void loop()
{

}
