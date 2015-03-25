# midi-dot-net
Automatically exported from code.google.com/p/midi-dot-net

Copyright © 2009 Tom Lokovic 

URL: ```http://code.google.com/p/midi-dot-net/ ```

Original description from http://code.google.com/p/midi-dot-net/ 

```wiki

Overview

This .NET library provides convenient, threadsafe access to MIDI devices. It does this by binding to the Win32 API with P/Invoke and then wrapping that in an object-oriented API which feels right at home in C# / .NET.

For a taste of what the API offers, check out the example snippets.
Features

    MIDI
        Easy access to MIDI input and output devices.
        Register input handlers using C# events / delegates.
        Full support for sending and receiving Note On, Note Off, Control Change, Program Change, and Pitch Bend messages.
        Convenient enums for General MIDI Channels, Pitches, Instruments, Controls, and Percussions. 
    Scheduling
        A powerful scheduler that lets you schedule MIDI messages, pause, unpause, and adjust beats-per-minute while it runs.
        Support for callback messages, so you can schedule call-outs to your own code at specific instants. Callback messages are scheduled just like MIDI messages, so they are subject to pause, unpause, and beats-per-minute as well.
        Callback messages can schedule additional messages when triggered (self-propagating messages), which allows for a flexible continuation-passing style of control.
        Built-in NoteOnOffMessage schedules the Off message when the On message triggers. 
    Music Theory
        Octave-independent Note class which differentiates among enharmonic variants (eg, D♯; and E♭). Notes can be resolved to specific pitches as needed.
        Scale class built from tonic note and ascent pattern. Includes built-in patterns (Major, Melodic Minor Ascending, Chromatic, etc).
        Chord class built from tonic note, ascent pattern, and inversion. Includes built-in chord patterns (Major, Seventh, Diminished, etc). 
    Documentation
        Interactive demo programs, both console and GUI.
        Comprehensive API documentation.
        Unit tests. 

Not-Yet-Features

    No support for extended MIDI messages such as System Exclusive ("sysex") messages.
    No MIDI file I/O. 

Requirements

    .NET Framework 3.5.
    Visual Studio C# 2008 (Express or Professional) or later.
    winmm.dll, the Win32 multimedia API which is standard on all modern Windows installs. 

Downloads

Source and binary distributions are available in the Downloads section.
	
Copyright © 2009 Tom Lokovic 

```


## LICENSE

New BSD License (The BSD 3-Clause License)

```
THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. 
IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, 
WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, 
EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```
