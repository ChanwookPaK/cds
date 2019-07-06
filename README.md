# cds

```cpp
void setup()  {

Serial.begin(9600);

void loop()   {
int top_left,top_right,bot_left,bot_right;
float top,bot,left,right;

top_left=analogRead(A0);
top_right=analogRead(A1);
bot_left=analogread(A2);
bot_right=analogread(A3);

top = (top_left+top_right)/2.0;
bot = (bot_left+bot_right)/2.0;
left = (top_left+bot_left)/2.0;
right = (top_right+bot_right)/2.0;

Serial.print("top_left=");Serial.println(top_left);
Serial.print("top_right=");Serial.println(top right);
Serial.print("bot_left=");Serial.println(bot left);
Serial.print("bot_right=");Serial.println(bot right);

}
