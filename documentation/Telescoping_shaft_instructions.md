# Telescoping torque shaft

The concept of a delta printer is to keep the effector as light as possible to avoid having too much mass and inertia at the print head. However extrusion of filament based systems is proven to be more efficient for multiple parameters when the drive of the filament is closer to the hotend - generally referred to as direct-drive systems.

Mechanically, there is no obligation to have the motor and the filament drive gears in the same location. It is done out of convenience and simplicity, but at the cost of weight. Even a pancake NEMA17 will weight a significant amount.

By keeping the drive gear on the effector but moving the motor off of it, we retain the main advantage of the delta printer of a light effector, but we also keep the filament drive near the hotend. I dub this concept (not entirely accurately): remote direct drive extrusion.

The key for a delta effector to do this effectively is to have a torque transmission that is as slop-free as possible, yet allows for a full range of motion of the effector. The telescoping torque shaft is my approach to doing so.

## Limitations

The shaft will need to use a double-u joint on each end, and telescope a significant amount. For the Monster Kossel project, I've had to do a triple-joint telescoping shaft to get the minimum length (when the hotend is at its home position - top of the print volume), and reach every part of the build plate (full extension). The length differential was close to a factor of 2.8 or 2.9. Depending on how tall you build the printer, that factor may change significantly. If it reaches above 3, you will need a 4-part telescoping shaft. If it drops to slightly less than 2, you can do it as a 2-part shaft.

Also my local experiments have shown that it works best if the driving motor shaft is placed such as to minimize the maximum angle that is required for printing. That is generally reached when the effector is at max printable height on the farthest side of where the motor is mounted. Thus, mounting the motor in the center would be most effective. However, I intend on having an air filter assembly in the center of the top frame. So mounting it in the middle of one of the top extrusions is the next best option.

The double-u joints will bring on a noticeable increase in effort for rotation above 30 degrees of axle transmission.

## Measuring the dimensions

The way the telescoping shaft works is by looking at what the minimum and maximum lengths should be across the print volume range of motion.

As indicated in the limitations section, the maximum extension is when the print head is at the opposite end of the horizontal, and at the build plate. Call this ***Lmax***.

The minimum extension will be at the upper-most printing height underneath the motor mount. This will be ***Lmin***.

If 3x ***Lmin*** > ***Lmax*** > 2 x ***Lmin***, then you will need a 3-segment telescoping. Keep in mind that there will be a minimum fixed distance added by each segment.

Consider the case where ***Lmin*** is 450mm and ***Lmax*** is 950mm. In that case your segment's maximum length is not going to be 450mm. Instead if will be closer to 430 or even 420mm length, because of the 4mm steel pins onto which the double-u joints attach on either end of the shaft.

The maximum extension, then, is not 430mm x 3 = 1290mm. The segments need to keep between 30 and 40mm of overlap, to transmit torque and keep proper alignment. So the calculation then returns: 3x (430-40) = 3x 390 = 1170mm. Still plenty given the distance of 950mm required.

## Assembly considerations

My prototype shaft uses 3 square aluminum tubing segments of nearly matching inner and outer sizes. The 7.5mm external tubing fits with about 0.5mm of tolerance in the 11.5mm external tubing (wall thickness is 1.5mm). I glued small felt pads on the ends of the rear of the 7mm segment, and the inside front of the 11.5mm segment. They are super-glued in place. To further smooth the motion, I added some PTFE grease. The 11mm segment also has felt pads super-glued to the rear of its segment. It then fits inside a 15.5mm segment where the front has pads on the inside, and the back is drilled for an M3x20 screw to go through and lock the printed cap in which the 4mm dowel attaches.

The 0.5mm gap is frustratingly small for the felt pads, as the thinnest I could find was closer to 1mm. However it compresses nicely and the PTFE grease lets it slide in without too much hassle or damage.

To guarantee proper telescoping operations, as well as avoiding getting grease on the filament's PTFE tube, I recommend attaching the outer-most segment to the effector, and the inner-most one to the motor. The reason for this is that gravity will be such that the inner-most tube will always extend fully first, before pulling the inner-most segment up. And conversely when it's being shrunk as the print head shrinks the distance, the first to start retracting will be pulled by gravity.