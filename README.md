# Josh Kannemeyer

Robotics software and applied AI. I build autonomous systems, and the tooling that makes building them less painful.

Essen, Germany · open to robotics / autonomy / AI roles (EU, remote or on-site) · [LinkedIn](https://www.linkedin.com/in/josh-kannemeyer/)

---

## What I do

I'm a robotics engineer with a master's in Automation & Robotics from TU Dortmund. Most of my work is where software meets hardware: getting a robot to work out where it is, plan a move, and actually follow it. I write the C++ and Python that has to keep doing that reliably.

The last couple of years I've built a lot with AI agents too. I run most of my own life through agents I've written, and I've built agent tooling for dev work. I don't let it run blind: the model drafts, I review, and I put hard checks around anything that matters. That habit of not trusting the output until it's verified is the same one you want in anything that moves in the real world.

## What I care about

Path planning and following. This is the part I keep coming back to. Holding a path when the sensors are noisy and the ground isn't flat is a genuinely hard problem, and I like working on it.

Autonomy that holds up outside the lab. GPS that drops out, a wheel that slips, a robot that has to keep going anyway. I'd rather get something working on real hardware than have it look perfect in sim.

Reliable AI. Verification-first, with hard checks where a wrong answer has a physical cost. "Usually right" stops being good enough once something can run into a wall.

Tooling that helps whoever's around me. If I work out something useful, I write it up or turn it into a script so the rest of the team gets it too. At my last job I gave an internal talk on the AI workflow I'd built.

## Robotics work

**[b.ob](https://github.com/lukasholtkamp/b.ob)** — Differential-drive robot on ROS2 Humble and a Raspberry Pi 4. Main contributor by commits (177 of 213). I built the assisted-driving side: a C++ lateral controller that holds the robot's heading on a path (PID on heading error, running off EKF-fused odometry, with angle wrapping and anti-windup so it doesn't fight itself), Lidar SLAM for mapping, and IMU + wheel-encoder localisation through an EKF. Autonomous navigation is the repo's next step.

**Master's thesis (Bertrandt)** — Trained a neural network to imitate an NMPC path-follower on a mobile robot, cutting the compute cost while keeping the tracking accuracy. C++ and Python on ROS2, IMU + Lidar fusion, tested in Gazebo and on the real robot.

**[Quadcopter](https://github.com/Desmondfotock28/Quadcopter)** — Contributor on an open-source C++ quadcopter project. Docs, repo structure, build-system cleanup.

## Also building

**Life OS** *(personal, ongoing)* — I run my life through a set of Claude agents: quests, calendar, planning, weekly reviews. Under the hood it's a folder layout and a library of skills I designed so the agents find the right context fast. Hooked into Apple Reminders, Google Calendar, and Google Workspace. Borrowed the idea from Karpathy's personal wiki.

**Job Search Control Center** — An agent pipeline I built to weigh up real openings. It scores how well a posting matches a profile, then drafts tailored application material from your actual history. Nothing auto-sends; every draft is for review. Runs locally on a Claude Code subscription.

## Next

Getting closer to the model itself. Running things locally, fine-tuning smaller models for specific tasks, and actually understanding what happens under the API call instead of wrapping a prompt around it.

## Stack

Core: C++, Python, ROS2, sensor fusion, Linux, Raspberry Pi.
Also: Claude Agent SDK, FastAPI, Bash, Docker, Django, React, PostgreSQL.
If I do something twice, it gets a script.
