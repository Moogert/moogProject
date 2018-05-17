# repair log
### contains everything i did and remembered to write down

## January 26th, 2016

Today I met with Dr. Bill Seaman to discuss interfaces with the Moog upon its
restoration. The meeting lasted about an hour, and touched on a wide variety of
possible approaches to the project. Dr. Seaman encouraged further contact should
I have any further questions.

Today's emphasis was on the Moog's power supply. (Without electricity, there
is no synth, and the rest of one's efforts are rendered moot.) Various parties were
contacted to ascertain a means of evaluating the PSU's functionality. Original
documentation was consulted for optimal voltage outputs.

Further interfaces between the Moog and the Seaboard Roli were briefly investigated.

~Jeffrey Wubbenhorst


## February 3rd, 2016

Today, I opened up the modular unit and pulled the 905 reverb unit and the 904-A low-pass filter out.
These modules are crucial to the Moog's sound, and the process of troubleshooting is reasonably well-documented.

The spring reverb has some issues with it. See this YouTube video for a demo:

https://youtu.be/1gt5yhT7iTA

I will confer with some folks on various forums and see if there are any solutions out there.

## February 3rd, 2016

I've fallen behind a bit on the logs. Things have been progressing; I now have:

* An oscilloscope, soldering station, frequency generator, and other tools to proceed with repairs and quantitative analysis. Quantitative analysis through technical means is preferred, since (for a filter, for example) it is preferable to be able to view on a time-based frequency spectrum chart than to say "well, it doesn't seem to sound right."

* I have been in contact with the manufacturers at Roli about implementing their product (Roli Rise) as an interface. They have provided technical advice on possible implementations; this advice will be evaluated over the next few days and contextualized for this project (there are some differences between the voltage standards that may need to be reconciled).

* Progress is being made on the online update system- there have been a few setbacks but I hope to have this up and running very soon.


## February 4th, 2016

Spent time evaluating the Moog's left 901-B module. Attached an oscilloscope to the oscillator's outputs and evaluated it from the perspective of a function generator.

The module itself does seem to generating reasonably (from a visual perspective) accurate waveforms, but acoustically, the unit is in need of significant repairs.

I also played the oscillator module through a speaker- there were significant instabilities in tuning, leading to a very unpleasant sound. Diagnostics are forthcoming.

I also communicated with some people online about the reverb unit. The advice I received was to replace the pots, as well as possibly replace the electrolytic caps.

I also talked with Prof. Stacy Tamtum from ECE about the project. I will be in communication with some potential advisors in the coming days.

All things considered, a very productive day.


A YouTube link to both videos is below:

https://www.youtube.com/watch?v=e0c7Rg4uEAg

https://www.youtube.com/watch?v=aBhi3mgZop4


## February 12th, 20116

Things have been busy. (I got sick, and was battling a lot of fatigue.)

I'm back in the saddle now, and went through all the documentation that I have
on file. I found out that the system we have is a 1968 modular system ("Synthesizer
1"), which is primarily an educational model. It's not designed to map out the sonic
universe in great detail, which explains a good bit of its functionality, but it is
still a good synth.

I looked into the keyboard controller for the Moog; I think it should be reasonably
straightforward to test its functionality. There is a tuning module that we might be
able to emulate using digital means. (Though, honestly, I think we should just focus
on getting more up-to-date interfaces for this thing.)

Most of the work done today related to getting documentation sorted out.

~Jeffrey


## February 19th, 2016

Met with Martin Brooke (faculty in ECE department) today- discussed
the power supply at length. Determined that a fuse was broken (may or
may not have been blown), will need to replace both fuse and fuse holder.

Prof. Brooke was optimistic about project, estimated that restoration
process will be relatively straightforward.

Power supply should be in good condition, can't say for sure right now.

Suggested going through synth linearly, starting with oscillators and
moving through towards everything else. This seems to be a good way
of doing things, and (now that the power supply is fixed) I think
that is the plan I will adopt.



## January 27th, 2016

Investigated the power supply, made contact with organizers of ECE Undergraduate Laboratory
for equipment and expertise. Had a discussion with Andrew Diao about approaches to evaluating
PSU's reliability. A meeting will likely be set up to make a more formal evaluation within the
next week.

Queries were also made regarding empirical studies on human interactions with electronic
instruments. While these studies are unlikely to play the largest part in the project's
evolution, they will likely be helpful. An inquiry was also made to Small Town Records (Duke's
record label) regarding the final musical result of this project.

## February 25th, 2016

Today I changed out the fuse and fuse holder, and obtained some
more tools for the project. upon changing the fuse, the CV routing
modules began to function, which was a great improvement. I wonder
what else works as a result of this repair (who can say I suppose).

One issue I'm having is that power does not seem to be delivered to
the oscillator section. I suspect that this is an internal wiring
problem, though it seems curious that this began since the beginning
of repairs.


## February 26th, 2016

Today I sought out advice as to why the oscillator section was not working.
The fact that the oscillators don't work after working previously is rather
odd, though I suspect that there's a reasonably straightforward solution.

Took a look at wiring diagrams, not sure what's wrong.


## February 29th, 2016

Emailed Justin Miles (ECE lab manager) about getting access to a power
soruce while the Moog's is being troubleshot. Posted to forums about
finding a solution to present issues.

Measured voltage to modules, 0V on all measurements taken. I honestly
have no idea why this is the case, will be moving forward on different
fronts while this gets sorted out. The rationale for replacing the
power source becomes stronger by the way (though it should be noted that
this is offset by the nightmare that rewiring everything would be).

I expect to have a Gantt chart for this project completed soon.

More soon.

~Jeffrey



## March 1st, 2016

Today I obtained a power supply from Justin Miles in ECE. IF all goes
according to plan, this will allow me to construct a test rig for the
Moog, which will let me get around the power supply issue for the time
being.

The forums have proved useful- from one anonymous Internet entity known
only by the moniker "robotmakers:"

++

I've modified Bel Power / Power One supplies to produce all the voltages in two vintage Moog systems, and the results are excellent. Hum is reduced - even proximity induced hum in the 905 reverbs is reduced/eliminated. Supply voltage variation is minimized which should also help tuning.

Highly recommended, even if the old supplies can be repaired. Just one resistor in each of the supplies needs to be replaced with a jumper, and you'd get the +12v, -10v and -6v you need. In addition, because the -10v is regulated (unlike the vintage Moog supply), you can add a few modern modules to the system. For example, I run some Moon modules in one Moog system off the +12v/-10v supply without issue.

HB5-3/OVP-AG supply normally provides 5V @ 3A. By replacing R7 with a jumper, you can dial in -6V with the trimmer potentiometer

HBB15-1.5-AG supply normally provides +/-12V @ 1.7A. By replacing R27 with a jumper, you can dial in -10V in addition to the +12V

Cheers,
Roger

++

link at:

https://www.muffwiggler.com/forum/viewtopic.php?t=156822

the HB5-3/OVP-AG power supply runs at about $60- the HBB15-1.5-AG supply runs about $80.
It would seem that replacing the power supply, while certainly not the most convenient
option, would certainly be an option not entirely outside the scope of this project.


## March 4th, 2016

Today was a productive day. Met with Martin Brooke, troubleshot power supply.
Established that transformer does indeed still work, issue most likely lies
blown capacitors (surprised they didn't blow earlier- par for the course,
really).

removed power supply, opened it up, cataloged and observed. PSU is not extraordinarily
complex, but there's work to be done for sure. Will probably source transistors
and diodes soon (full reconstruction isn't the worst thing that could happen).

Internal wiring of Moog is a mystery; I have no schematics , meaning that any
info will be deducted from our specific model.

I cataloged all the capacitors we have, and will begin sourcing those soon.
Meanwhile, I'm trying to work out a good way to make a makeshift power supply
to troubleshoot individual components. Will send some more emails on this.

Things are looking good, but there's work to do.

~Jeffrey


## March 5th, 2016

Got a response from @robotmakers on the Muffwiggler.com forums. Explained how to
install a Bel-Power power supply cheaply and easily. ("Cheap" being a relative
term here..." A link to the discussion is below, but I think that this is
honestly going to be the best option for the time being:

https://www.muffwiggler.com/forum/viewtopic.php?p=2165399#2165399

going to see if I can get bench power supply to power the synth for the
time being. May work with Jason Kim on this to prevent the electrocution of
myself or the destruction of poor Misty.

All for now. More later.

~Jeffrey

## March 15th, 2016

Figured out a makeshift power supply. Tested oscillator module, got a hideous crackling. Noise
grenerator works Ok. Will begin evaluation of synth's functionality soon.  

## March 18th, 2016

Ordered capacitors and Bel-power power supplies from ECE parts request website.
Sent an email about the authenticity of 901-B oscillators, trying to ascertain
what components should be replaced with abandon, if I should try and hold out
for anything vintage. (Odds are I'll just try and order new parts, but I figure
it's worth asking.)

Have been absent in part due to illness. (Food poisoning is no fun.)


## March 24th, 2016

Today I talked more about getting parts ordered. Looking into getting the
950 restored (which is not the biggest of my worried right now, though it
would be good to get access to some kind of MIDI-CV converter soon so I
can test the oscillators soon).

Next up is to reconcile trigger voltages (hopefully with eurorack).

i need to sleep

~Jeffrey


## March 26th, 2016

Finally got capacitors ordered. Should arrive pretty soon. Going to try and reconcile
Moog and eurorack trigger standards (goal is to not blow anything up).

### UPDATE: [though technically this should be in the logs as the 27th]

found some more resources on trigger standards, sent an email to synthesizers.com
folks to see what they think about buying their product. I've got a pretty good
shot (IMO) of successfully reconciling the Moog standards with the Eurorack
standards (assuming that they differ in any significant ways, I think there's
actually going to be more overlap than I originally thought).

strongly considering constructing (as a Eurorack module) a converter
that deals with gate + CV if I end up needing it. (because I'm not sure I'll need it
in the end). another wild saturday night

More soon. At an engineering conference. #sobriety

~Jeffrey


## March 29th, 2016

OK, so today was a good day. I hooked up the power source correctly (bench power)
and plugged in the oscillators. I got noise (!), which was very encouraging,
and made me very happy. (A video of me screaming like a 5-year-old at the glorious
noise of three stacked oscillators can be found at https://www.youtube.com/watch?v=-KOKWHhS9V0 )

Tested filter bank; some filter bands don't work. Will ask why online (I suspect broken pots?).

1000, 2800, 500, bands on the filter bank are not functional. I suspect bad pots, will get to
cleaning those soon. It's been a good day.

~Jeffrey

## March 30th, 2016

Tested VCAs with Dewey Lawson. Both VCAs seem to work, no significant issues observed.
Both linear and exponential model work, all CV inputs seem to perfom perfectly. As a
side note, the amplifiers seem to overdrive very nicely, giving some very pleasing
lower frequencies. (Not sure if that's overdrive or normal behavior, but it sounds like
overdrive, so I shall, for the moment, term is as such.)

Power issues are still keeping me from figuring out the envelope generator, but I think
that should be resolved soon.

Pots need to be cleaned for both VCAs, but I don't think that's going to be an issue.

Low-pass filter is no longer functional, no idea why. Details to follow.

Good day. Here's to more like it.

~Jeffrey

## April 4th, 2016

Determined possible expenditures to upgrade/repair Moog. $$$ are an adventure indeed....



# April 7th, 2016

Cleaned out most of the potentiometers today. There are a few modules I have left to do,
and there are a number of potentiometers that we should just replace altogether. These are
documented in the "potentiometers.md" file.



## April 23rd, 2016

Been a while since I've done any documentation; health issues plauged me since the 8th but (praise God)
that's over with now. Seems like I've spent the better part of this week sending emails related to this
project (instead of actually soldering things).

At any rate- I'm working on sourcing switches for the 'From 2' switch on the CV routing section.
It ain't cheap, that's for sure.

working on securing studio time. Trying to get people to buy me fancy gear for recording.

One recent development is the possible failure of the filter bank's capacitors, which would
be responsible for the filter's hissing (which I need to evaluate again, by the way).

Thread: http://forum.moogmusic.com/viewtopic.php?f=18&t=25380

I'm making a list of possible potentiometers to replace, any orders that are going to take
place need to happen soon.

working on calibrating VCAs, unfortunately the old PCB systems weren't labeled, so
I've been spending (perhaps more than I'd planned) some time trying to trace out the
PCB to figure out where to put meters and things. (Also trying to figure out what trim-pot
does what...)

Good times. More to come. Things are starting to heat up.

~Jeffrey

## April 26th, 2016

Sending emails right and left. Moog Music has very graciously donated (lent, really) some sweet CV-controlling
gear (as well as some other goodies :) to the project, so I'm looking forward to that with great excitement.

Sourcing parts, planning on making a final order today or tomorrow. Filing for all sorts of grants and things,
trying to get enough sleep/finish all the other school stuff that needs to be done. Talking with recording
studio to try and set up logistics; realizing I've never heard Misty (as it's been dubbed) on nice speakers.

UPDATE: I ordered $100 or trigger cables/converters, bought the Bel-power units (at last) for some nice,
clean power. Will work on potentiometer stuff tomorrow morning, I think.

...and that's about it. More later.

~Jeffrey



## May 13th, 2016

...For starters, I'm behind on documentation. Things that have transpired:

* I made the Moog work with the eurorack standard! It's not a Eurorack module by any stretch of the imagination, but I can output trigger voltages ('gate' in modern parlance) and CV into the Moog and get pitches out of it.

* The PSU now works! (whee). It's taken way too long to get reliable power into this thing...

* I've placed an order for parts and things (mostly potentiometers), which should greatly improve Misty's tactile response and reliability. Calibration has been temporarily postponed until parts get in (which just seems to make sense to me.)

* I'll be presenting the Moog at Moogfest- the cool thing is, the Moog doesn't actually have to make noises during this time, which makes my life much easier (I was preparing for a full audio demo, which was starting to make life look something other than tranquil)

* The Moog is now MIDI-compliant (yee), courtesy of the Expert Sleepers FH-1 and the Fakhoury family (thx so much you guys, I really don't know how to thank you). There's another MIDI-CV converter coming in soon (thanks to the Innovation Co-Lab at Duke), though that has yet to be implemented  

* I also "repaired" (zip-tied) the 950 keyboard controller into a cohesive unit (stuff was flopping all over the place inside of it). This is not a permanent solution, but should suffice for the time being.

...I think that's about all. Documentation is often correlated to free time (or a lack thereof).

~Jeffrey
