# Ex09 Event Registration Web Application
# Date:08.10.2025
# AIM:
To design, develop and deploy a web application for event registration.

# DESIGN STEPS:
## Step 1:
Create a new frame.

## Step 2:
Select any one preset size of your choice.

## Step 3:
Select the shapes you need.

## Step 4:
Import images as needed.

## Step 5:
Create pages based on your need and link them.

## Step 6:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# DESIGN TOOL:
Figma

# CODE:
```
page 1

import React from "react";
import background1 from "./background-1.png";
import logo11 from "./logo-1-1.png";
import rectangle1 from "./rectangle-1.svg";
import rectangle2 from "./rectangle-2.svg";

export const AndroidCompact = (): JSX.Element => {
  return (
    <main className="bg-white w-full min-w-[412px] min-h-[860px] relative">
      <img
        className="absolute top-0 left-0 w-[412px] h-[860px] aspect-[0.67] object-cover"
        alt="Background"
        src={background1}
      />

      <header className="absolute top-[45px] left-0.5 w-[406px] h-[61px]">
        <img
          className="w-full h-full aspect-[6.65] object-cover"
          alt="Logo"
          src={logo11}
        />
      </header>

      <div className="absolute top-[646px] left-[68px] [font-family:'Jim_Nightshade-Regular',Helvetica] font-normal text-white text-9xl tracking-[0] leading-[normal]">
        {""}
      </div>

      <h1 className="absolute top-[104px] left-[142px] w-[191px] [font-family:'Jim_Nightshade-Regular',Helvetica] font-normal text-[#060912] text-9xl tracking-[0] leading-[normal]">
        sec
      </h1>

      <h2 className="absolute top-[232px] left-[18px] [font-family:'Jim_Nightshade-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]">
        hostel fest&apos;25
      </h2>

      <nav
        className="absolute top-[360px] left-[120px] flex flex-col gap-[19px]"
        aria-label="Main navigation"
      >
        <a
          href="/login"
          className="relative w-[170px] h-[41px] flex items-center justify-center"
          aria-label="Login to your account"
        >
          <img
            className="absolute inset-0 w-full h-full"
            alt=""
            src={rectangle1}
          />
          <span className="relative [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-white text-xl tracking-[0] leading-[normal]">
            login
          </span>
        </a>

        <a
          href="/register"
          className="relative w-[170px] h-[41px] flex items-center justify-center"
          aria-label="Register for an account"
        >
          <img
            className="absolute inset-0 w-full h-full"
            alt=""
            src={rectangle2}
          />
          <span className="relative [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-white text-xl tracking-[0] leading-[normal]">
            register
          </span>
        </a>
      </nav>
    </main>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src//*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

page 2

import React from "react";
import screenshot202510070026461 from "./screenshot-2025-10-07-002646-1.png";

export const AndroidCompact = (): JSX.Element => {
  const culturalEvents = [
    "Mehendi",
    "Digital Art",
    "Makeup&Hairdo",
    "Drawing",
    "Ramp Walk",
    "Solo Dance",
    "Solo Singing",
    "Chinese Whisper",
  ];

  return (
    <div className="bg-white w-full min-w-[412px] min-h-[860px] relative">
      <img
        className="absolute top-0 left-0 w-[412px] h-[860px] aspect-[0.75] object-cover"
        alt="Screenshot"
        src={screenshot202510070026461}
      />

      <div className="absolute top-32 left-[26px] [font-family:'Jim_Nightshade-Regular',Helvetica] font-normal text-[#effdff] text-[64px] tracking-[0] leading-[normal]">
        cultural events....
      </div>

      <ul className="absolute top-[217px] left-[42px] [font-family:'Gluten-Regular',Helvetica] font-normal text-white text-2xl tracking-[0] leading-[normal] list-none">
        {culturalEvents.map((event, index) => (
          <li key={index} className="flex items-start">
            <span className="[font-family:'Gluten-Regular',Helvetica] font-normal text-white text-[64px] tracking-[0] leading-[1]">
              .
            </span>
            <span className="text-2xl leading-[normal]">
              {event}
              <br />
            </span>
          </li>
        ))}
      </ul>
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src//*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

page 3

import React, { useState } from "react";
import image from "./image.svg";
import rectangle3 from "./rectangle-3.svg";
import rectangle4 from "./rectangle-4.svg";
import rectangle6 from "./rectangle-6.svg";
import rectangle7 from "./rectangle-7.svg";
import screenshot202510070048291 from "./screenshot-2025-10-07-004829-1.png";
import vector from "./vector.svg";

export const AndroidCompact = (): JSX.Element => {
  const [formData, setFormData] = useState({
    name: "",
    age: "",
    gender: "",
    registerNo: "",
    department: "",
    mobileNo: "",
  });

  const handleInputChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    const { name, value } = e.target;
    setFormData((prev) => ({
      ...prev,
      [name]: value,
    }));
  };

  const handleSubmit = (e: React.FormEvent) => {
    e.preventDefault();
    console.log("Form submitted:", formData);
  };

  return (
    <div className="bg-white w-full min-w-[412px] min-h-[860px] relative">
      <img
        className="absolute top-0 left-0 w-[412px] h-[860px] aspect-[1.58] object-cover"
        alt="Screenshot"
        src={screenshot202510070048291}
      />

      <header className="absolute top-[34px] left-[49px] [font-family:'Jim_Nightshade-Regular',Helvetica] font-normal text-white text-[40px] tracking-[0] leading-[normal]">
        Event Registration Form
      </header>

      <form onSubmit={handleSubmit} className="relative">
        <div className="absolute top-[153px] left-[37px] w-[344px] h-[38px]">
          <img
            className="absolute top-0 left-0 w-full h-full"
            alt="Name field background"
            src={vector}
          />
          <label
            htmlFor="name"
            className="absolute top-[-13px] left-[12px] w-[91px] [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-white text-xl tracking-[0] leading-[normal]"
          >
            Name:
          </label>
          <input
            type="text"
            id="name"
            name="name"
            value={formData.name}
            onChange={handleInputChange}
            className="absolute top-0 left-0 w-full h-full px-3 bg-transparent text-white [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-base tracking-[0] leading-[normal] focus:outline-none focus:ring-2 focus:ring-white focus:ring-opacity-50"
            aria-label="Name"
            required
          />
        </div>

        <div className="absolute top-[225px] left-[37px] w-[344px] h-[38px]">
          <img
            className="absolute top-0 left-0 w-full h-full"
            alt="Age field background"
            src={rectangle4}
          />
          <label
            htmlFor="age"
            className="absolute top-[-13px] left-[12px] w-[91px] [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-white text-xl tracking-[0] leading-[normal]"
          >
            Age:
          </label>
          <input
            type="number"
            id="age"
            name="age"
            value={formData.age}
            onChange={handleInputChange}
            className="absolute top-0 left-0 w-full h-full px-3 bg-transparent text-white [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-base tracking-[0] leading-[normal] focus:outline-none focus:ring-2 focus:ring-white focus:ring-opacity-50"
            aria-label="Age"
            required
          />
        </div>

        <div className="absolute top-[305px] left-[37px] w-[344px] h-[38px]">
          <img
            className="absolute top-0 left-0 w-full h-full"
            alt="Gender field background"
            src={rectangle3}
          />
          <label
            htmlFor="gender"
            className="absolute top-[-13px] left-[12px] w-[120px] [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-white text-xl tracking-[0] leading-[normal]"
          >
            Gender:
          </label>
          <input
            type="text"
            id="gender"
            name="gender"
            value={formData.gender}
            onChange={handleInputChange}
            className="absolute top-0 left-0 w-full h-full px-3 bg-transparent text-white [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-base tracking-[0] leading-[normal] focus:outline-none focus:ring-2 focus:ring-white focus:ring-opacity-50"
            aria-label="Gender"
            required
          />
        </div>

        <div className="absolute top-[385px] left-[37px] w-[344px] h-[38px]">
          <img
            className="absolute top-0 left-0 w-full h-full"
            alt="Register number field background"
            src={image}
          />
          <label
            htmlFor="registerNo"
            className="absolute top-[-13px] left-[12px] w-[220px] [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-white text-xl tracking-[0] leading-[normal]"
          >
            Register No.:
          </label>
          <input
            type="text"
            id="registerNo"
            name="registerNo"
            value={formData.registerNo}
            onChange={handleInputChange}
            className="absolute top-0 left-0 w-full h-full px-3 bg-transparent text-white [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-base tracking-[0] leading-[normal] focus:outline-none focus:ring-2 focus:ring-white focus:ring-opacity-50"
            aria-label="Register Number"
            required
          />
        </div>

        <div className="absolute top-[465px] left-[37px] w-[344px] h-[38px]">
          <img
            className="absolute top-0 left-0 w-full h-full"
            alt="Department field background"
            src={rectangle6}
          />
          <label
            htmlFor="department"
            className="absolute top-[-13px] left-[12px] w-[216px] [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-white text-xl tracking-[0] leading-[normal]"
          >
            Department:
          </label>
          <input
            type="text"
            id="department"
            name="department"
            value={formData.department}
            onChange={handleInputChange}
            className="absolute top-0 left-0 w-full h-full px-3 bg-transparent text-white [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-base tracking-[0] leading-[normal] focus:outline-none focus:ring-2 focus:ring-white focus:ring-opacity-50"
            aria-label="Department"
            required
          />
        </div>

        <div className="absolute top-[545px] left-[37px] w-[344px] h-[38px]">
          <img
            className="absolute top-0 left-0 w-full h-full"
            alt="Mobile number field background"
            src={rectangle7}
          />
          <label
            htmlFor="mobileNo"
            className="absolute top-[-13px] left-[10px] w-[226px] [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-white text-xl tracking-[0] leading-[normal]"
          >
            Mobile No,:
          </label>
          <input
            type="tel"
            id="mobileNo"
            name="mobileNo"
            value={formData.mobileNo}
            onChange={handleInputChange}
            className="absolute top-0 left-0 w-full h-full px-3 bg-transparent text-white [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-base tracking-[0] leading-[normal] focus:outline-none focus:ring-2 focus:ring-white focus:ring-opacity-50"
            aria-label="Mobile Number"
            required
          />
        </div>

        <button
          type="submit"
          className="absolute top-[647px] left-[100px] w-[219px] h-12 bg-[#335c83] hover:bg-[#2a4d6d] active:bg-[#1f3a52] transition-colors duration-200 focus:outline-none focus:ring-2 focus:ring-white focus:ring-opacity-50"
          aria-label="Register for event"
        >
          <span className="absolute top-[11px] left-[36px] [font-family:'Gravitas_One-Regular',Helvetica] font-normal text-white text-xl tracking-[0] leading-[normal]">
            REGISTER
          </span>
        </button>
      </form>
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src//*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

page 4

import React from "react";
import background1 from "./background-1.png";
import logo11 from "./logo-1-1.png";

export const AndroidCompact = (): JSX.Element => {
  return (
    <main className="bg-white overflow-hidden w-full min-w-[412px] min-h-[860px] relative">
      <img
        className="absolute top-0 left-0 w-[412px] h-[860px] aspect-[0.67] object-cover"
        alt="Background with blue lighting and crowd silhouettes"
        src={background1}
      />

      <header className="absolute top-[45px] left-0.5 w-[406px] h-[61px]">
        <img
          className="w-full h-full aspect-[6.65] object-cover"
          alt="Sayeetha Engineering College Autonomous TNEA Code 1216 logo"
          src={logo11}
        />
      </header>

      <section
        className="absolute top-[182px] left-8 w-[460px]"
        aria-labelledby="thank-you-heading"
      >
        <h1
          id="thank-you-heading"
          className="[font-family:'Jim_Nightshade-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]"
        >
          THANK YOU
        </h1>
      </section>

      <section
        className="absolute top-[303px] left-8 w-[536px]"
        aria-labelledby="event-message"
      >
        <p
          id="event-message"
          className="[font-family:'Gluten-Regular',Helvetica] font-normal text-black text-2xl tracking-[0] leading-[normal]"
        >
          &nbsp;&nbsp; We are all eagerly waiting
          <br />
          for your participation in the
          <br />
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;cultural
          events
        </p>
      </section>

      <section
        className="absolute top-[407px] left-[17px] w-[411px]"
        aria-labelledby="contact-info"
      >
        <address className="not-italic">
          <p
            id="contact-info"
            className="[font-family:'Gravitas_One-Regular',Helvetica] font-normal text-[#141111] text-2xl tracking-[0] leading-[normal]"
          >
            CONTACT US:
            <br />
            PHONE NO.{" "}
            <a href="tel:1234567890" className="hover:underline">
              12345 67890
            </a>
          </p>
        </address>
      </section>
    </main>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src//*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}
```
# OUTPUT:
![alt text](event.jpg)
# RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
