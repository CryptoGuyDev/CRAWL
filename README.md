<!-- PROJECT LOGO -->
<p align="center">
  <h3 align="center">Crawl (CryptoGuy)</h3>

  <p align="center">
    The open-source Calendly successor.
    <br />
    <a href="https://kingscord-official.vercel.app/"><strong>Learn more »</strong></a>
    <br />
    <br />
    <a href="https://discord.gg/BgeGHvydwM">Discord</a>
    ·
    <a href="https://kingscord-official.vercel.app/">Website</a>
    ·
    <a href="https://github.com/CryptoGuyDev/kingscord/issues">Issues</a>
  </p>
</p>

<p align="center">
   <a href="https://discord.gg/BgeGHvydwM"><img src="https://img.shields.io/badge/Discord-go.cal.com%2Fdiscord-%234A154B" alt="Join Crew.com Discord"></a>
   <a href=""><img src="https://img.shields.io/badge/Product%20Hunt-%231%20Product%20of%20the%20Month-%23DA552E" alt="Product Hunt"></a>
   <a href=""><img height="20px" src="https://betteruptime.com/status-badges/v1/monitor/a9kf.svg" alt="Uptime"></a>
   <a href=""><img src="https://img.shields.io/github/stars/calcom/cal.com" alt="Github Stars"></a>
   <a href=""><img src="https://img.shields.io/badge/Hacker%20News-%231-%23FF6600" alt="Hacker News"></a>
   <a href=""><img src="https://img.shields.io/badge/license-AGPLv3-purple" alt="License"></a>
   <a href=""><img src="https://img.shields.io/github/commit-activity/m/calcom/cal.com" alt="Commits-per-month"></a>
   <a href=""><img src="https://img.shields.io/badge/Pricing-Free-brightgreen" alt="Pricing"></a>
   <a href=""><img src="https://img.shields.io/docker/pulls/calendso/calendso"></a>
   <a href=""><img src="https://img.shields.io/twitch/status/calcomtv?style=flat"></a>
   <a href=""><img src="https://img.shields.io/badge/Help%20Wanted-Contribute-blue"></a>
   <a href=""><img src="https://img.shields.io/badge/Figma-Design%20System-blueviolet"></a>
   <a href=""><img src="https://img.shields.io/badge/translations-contribute-brightgreen" /></a>
   <a href=""><img src="https://img.shields.io/badge/Contributor%20Covenant-1.4-purple" /></a>
   <a href=""><img src="https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fcal%2Fbounties%3Fstatus%3Dopen" /></a>
</p>

<!-- ABOUT THE PROJECT -->

## About the Project

# Scheduling Meetings for absolutely everyone

The open source Meeting Source. You are in charge
of your own data, workflow, and appearance.

Personal Meetings And Scheduling Meetings are awesome. It made our lives massively easier. We're using it for business meetings, seminars, yoga classes, and even calls with our families. However, most tools are very limited in terms of control and customization.

### Built With

- [Next.js](https://nextjs.org/)
- [tRPC](https://trpc.io/)
- [React.js](https://reactjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Prisma.io](https://prisma.io/)

## Contact us

Meet our sales team for any commercial inquiries.

Email: cryptogfx.official@gmail.com

## Stay Up-to-Date

Crawl.com officially launched as v.1.0 on the 20th of April 2024 and we've come a long way so far. Watch **releases** of this repository to be notified of future updates.

<!-- GETTING STARTED -->

## <a name="quick-start">🤸 Quick Start</a>

Follow these steps to set up the project locally on your machine.

**Prerequisites**

Make sure you have the following installed on your machine:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/) (Node Package Manager)

**Cloning the Repository**

```bash
https://github.com/CryptoGuyDev/kingscord/tree/main
cd kingscord
```

**Installation**

Install the project dependencies using npm:

```bash
npm install
```

**Set Up Environment Variables**

Create a new file named `.env` in the root of your project and add the following content:

```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up

NEXT_PUBLIC_STREAM_API_KEY=
STREAM_SECRET_KEY=
```

Replace the placeholder values with your actual Clerk & getstream credentials. You can obtain these credentials by signing up on the [Clerk website](https://clerk.com/) and [getstream website](https://getstream.io/)

**Running the Project**

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to view the project.

## <a name="snippets">🕸️ Snippets</a>

<details>
<summary><code>app/globals.css</code></summary>

```css
@tailwind base;
@tailwind components;
@tailwind utilities;

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* ======== stream css overrides ======== */
.str-video__call-stats {
  max-width: 500px;
  position: relative;
}

.str-video__speaker-layout__wrapper {
  max-height: 700px;
}

.str-video__participant-details {
  color: white;
}

.str-video__menu-container {
  color: white;
}

.str-video__notification {
  color: white;
}

.str-video__participant-list {
  background-color: #1c1f2e;
  padding: 10px;
  border-radius: 10px;
  color: white;
  height: 100%;
}

.str-video__call-controls__button {
  height: 40px;
}

.glassmorphism {
  background: rgba(255, 255, 255, 0.25);
  backdrop-filter: blur(4px);
  -webkit-backdrop-filter: blur(4px);
}
.glassmorphism2 {
  background: rgba(18, 17, 17, 0.25);
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
}

/* ==== clerk class override ===== */

.cl-userButtonPopoverActionButtonIcon {
  color: white;
}

.cl-logoBox {
  height: 40px;
}
.cl-dividerLine {
  background: #252a41;
  height: 2px;
}

.cl-socialButtonsIconButton {
  border: 3px solid #565761;
}

.cl-internal-wkkub3 {
  color: white;
}
.cl-userButtonPopoverActionButton {
  color: white;
}

/* =============================== */

@layer utilities {
  .flex-center {
    @apply flex justify-center items-center;
  }

  .flex-between {
    @apply flex justify-between items-center;
  }
}

/* animation */

.show-block {
  width: 100%;
  max-width: 350px;
  display: block;
  animation: show 0.7s forwards linear;
}

@keyframes show {
  0% {
    animation-timing-function: ease-in;
    width: 0%;
  }

  100% {
    animation-timing-function: ease-in;
    width: 100%;
  }
}
```

</details>

<details>
<summary><code>tailwind.config.ts</code></summary>

```typescript
import type { Config } from 'tailwindcss';

const config = {
  darkMode: ['class'],
  content: [
    './pages/**/*.{ts,tsx}',
    './components/**/*.{ts,tsx}',
    './app/**/*.{ts,tsx}',
    './src/**/*.{ts,tsx}',
  ],
  prefix: '',
  theme: {
    container: {
      center: true,
      padding: '2rem',
      screens: {
        '2xl': '1400px',
      },
    },
    extend: {
      colors: {
        dark: {
          1: '#1C1F2E',
          2: '#161925',
          3: '#252A41',
          4: '#1E2757',
        },
        blue: {
          1: '#0E78F9',
        },
        sky: {
          1: '#C9DDFF',
          2: '#ECF0FF',
          3: '#F5FCFF',
        },
        orange: {
          1: '#FF742E',
        },
        purple: {
          1: '#830EF9',
        },
        yellow: {
          1: '#F9A90E',
        },
      },
      keyframes: {
        'accordion-down': {
          from: { height: '0' },
          to: { height: 'var(--radix-accordion-content-height)' },
        },
        'accordion-up': {
          from: { height: 'var(--radix-accordion-content-height)' },
          to: { height: '0' },
        },
      },
      animation: {
        'accordion-down': 'accordion-down 0.2s ease-out',
        'accordion-up': 'accordion-up 0.2s ease-out',
      },
      backgroundImage: {
        hero: "url('/images/hero-background.png')",
      },
    },
  },
  plugins: [require('tailwindcss-animate')],
} satisfies Config;

export default config;
```

</details>

<details>
<summary><code>components/MeetingCard.tsx</code></summary>

```typescript
"use client";

import Image from "next/image";

import { cn } from "@/lib/utils";
import { Button } from "./ui/button";
import { avatarImages } from "@/constants";
import { useToast } from "./ui/use-toast";

interface MeetingCardProps {
  title: string;
  date: string;
  icon: string;
  isPreviousMeeting?: boolean;
  buttonIcon1?: string;
  buttonText?: string;
  handleClick: () => void;
  link: string;
}

const MeetingCard = ({
  icon,
  title,
  date,
  isPreviousMeeting,
  buttonIcon1,
  handleClick,
  link,
  buttonText,
}: MeetingCardProps) => {
  const { toast } = useToast();

  return (
    <section className="flex min-h-[258px] w-full flex-col justify-between rounded-[14px] bg-dark-1 px-5 py-8 xl:max-w-[568px]">
      <article className="flex flex-col gap-5">
        <Image src={icon} alt="upcoming" width={28} height={28} />
        <div className="flex justify-between">
          <div className="flex flex-col gap-2">
            <h1 className="text-2xl font-bold">{title}</h1>
            <p className="text-base font-normal">{date}</p>
          </div>
        </div>
      </article>
      <article className={cn("flex justify-center relative", {})}>
        <div className="relative flex w-full max-sm:hidden">
          {avatarImages.map((img, index) => (
            <Image
              key={index}
              src={img}
              alt="attendees"
              width={40}
              height={40}
              className={cn("rounded-full", { absolute: index > 0 })}
              style={{ top: 0, left: index * 28 }}
            />
          ))}
          <div className="flex-center absolute left-[136px] size-10 rounded-full border-[5px] border-dark-3 bg-dark-4">
            +5
          </div>
        </div>
        {!isPreviousMeeting && (
          <div className="flex gap-2">
            <Button onClick={handleClick} className="rounded bg-blue-1 px-6">
              {buttonIcon1 && (
                <Image src={buttonIcon1} alt="feature" width={20} height={20} />
              )}
              &nbsp; {buttonText}
            </Button>
            <Button
              onClick={() => {
                navigator.clipboard.writeText(link);
                toast({
                  title: "Link Copied",
                });
              }}
              className="bg-dark-4 px-6"
            >
              <Image
                src="/icons/copy.svg"
                alt="feature"
                width={20}
                height={20}
              />
              &nbsp; Copy Link
            </Button>
          </div>
        )}
      </article>
    </section>
  );
};

export default MeetingCard;
```

</details>

## <a name="links">🔗 Links</a>
