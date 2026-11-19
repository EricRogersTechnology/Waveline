# Waveline — Support

A remote control for your software-defined radio: tune, listen, scan, record and decode Morse
from iPhone, iPad, Apple Watch and Apple TV.

**Need help?** Email [Eric@EricRogersTechnology.com](mailto:Eric@EricRogersTechnology.com)
and I'll get back to you. Including your device, iOS version, receiver model and SDRconnect
version helps me answer faster.

For TestFlight beta testers: you can also send feedback directly through the TestFlight
app. Take a screenshot, then tap **Send Beta Feedback**.

## Frequently asked

**What do I need?**
A compatible SDR receiver and a computer on your network (Mac, Windows PC, Linux PC or
Raspberry Pi) running SDRconnect with its WebSocket API turned on. Waveline is a remote
control: it doesn't contain a radio and can't receive anything on its own. To look around
first, tap **Try Demo Mode** on the first screen. It simulates a receiver with weather
stations, repeaters and a Morse beacon.

**How do I turn on SDRconnect's WebSocket API?**
For the headless SDRconnect server, start it with `--websocket_port=5454`, for example
`SDRconnect_headless --websocket_port=5454`. Waveline connects on port 5454 by default.

**How do I connect?**
On the first screen, tap **Find on This Network** to look for SDRconnect on your Wi-Fi, or add
the computer's IP address by hand. Then pick your receiver. Allow **Local Network** access
when iOS asks; Waveline can't reach SDRconnect without it. To change it later, go to
Settings → Privacy & Security → Local Network.

**It says SDRconnect isn't answering.**
The computer accepted the connection but SDRconnect didn't reply. Restart SDRconnect on that
computer, then try again.

**It says "View only — another app is controlling this receiver."**
Another app (or SDRconnect itself) is in control. Close the other client and reconnect.

**Can I use it away from home?**
Yes, with Tailscale. Install it on the SDRconnect computer and your iPhone, signed in to the same
account, then add a host in Waveline using the computer's **Tailscale name**: the short name shown
in the Tailscale app, such as `macbook-pro`. Use the name, not the 100.x address, because iOS only
allows this kind of connection to addresses it treats as local. Keep MagicDNS turned on in
Tailscale so the name works. Don't open SDRconnect's port on your router: Waveline can't use it
that way, and the API has no password. Audio uses about 1.5 Mbit/s (around 700 MB per hour).

**How do memories and scanning work?**
Tap ★ to save the frequency you're on, or import a channel list (CSV) from your radio's
programming software under **Memories → +**. Group channels into banks, then tap **Scan**.
The scanner stops on active channels. Use Hold, Skip and Stop in the banner. Turn on **Record
Each Hit** to save every stop as a recording.

**Where are my recordings?**
In the Files app, under **On My iPhone → Waveline → Recordings**. You can also play and share
them from **••• → Recordings**.

**What's on the Apple Watch?**
A remote for the iPhone app: tuning with the Digital Crown, Listen, Mute, Record, memories
and scanning. Keep Waveline connected on your iPhone, and the watch controls it.

**Does it work with Siri and Shortcuts?**
Yes: "Listen with Waveline", "Scan with Waveline", "Tune Waveline to…" and more. Listen, Scan and
Stop are also available as Control Center controls.

**Is it accessible?**
Waveline supports VoiceOver, Larger Text, Dark Mode, Reduce Motion, and text and controls meet colour-contrast guidelines. Live
Transcript turns voice into text, and the CW decoder turns Morse into text.

**Is my data private?**
Yes. There's no account, no ads and no tracking, and Waveline only talks to the computer you
connect it to. See the [Privacy Policy](PRIVACY.html).

---

© 2026 Eric Rogers Technology · [Privacy Policy](PRIVACY.html)
