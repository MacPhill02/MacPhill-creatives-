// Creative Innovation Group Website

import React from "react"; import { Button } from "@/components/ui/button"; import { Card, CardContent } from "@/components/ui/card"; import { Input } from "@/components/ui/input"; import { Textarea } from "@/components/ui/textarea"; import { Instagram, Mail, Phone, Tiktok } from "lucide-react"; import { motion } from "framer-motion";

export default function HomePage() { return ( <div className="min-h-screen bg-white text-black font-sans"> {/* Header */} <header className="bg-black text-white p-6 flex justify-between items-center shadow-md"> <h1 className="text-2xl font-bold">Creative Innovation Group</h1> <nav className="space-x-4"> <a href="#about">About</a> <a href="#join">Join Us</a> <a href="#work">Our Work</a> <a href="#blog">Blog</a> <a href="#contact">Contact</a> </nav> </header>

{/* Hero */}
  <section className="text-center py-20 bg-gradient-to-r from-indigo-500 to-purple-600 text-white">
    <motion.h2 className="text-4xl font-bold mb-4" initial={{opacity: 0, y: -20}} animate={{opacity: 1, y: 0}}>Innovate. Create. Inspire.</motion.h2>
    <p className="text-lg">We are a movement of dreamers building tomorrow through design, tech, and vision.</p>
  </section>

  {/* About Us */}
  <section id="about" className="py-16 px-8 max-w-4xl mx-auto">
    <h3 className="text-3xl font-semibold mb-4">About Us</h3>
    <p>
      Creative Innovation Group is a youth-led collective based in Botswana focused on
      turning bold ideas into practical solutions — from technology and fashion to sustainability and community impact.
    </p>
  </section>

  {/* Join Us */}
  <section id="join" className="py-16 px-8 bg-gray-100">
    <h3 className="text-3xl font-semibold mb-6">Join Us</h3>
    <p className="mb-4">Want to collaborate or become part of our mission? Fill in your info below:</p>
    <div className="max-w-xl mx-auto space-y-4">
      <Input placeholder="Full Name" />
      <Input placeholder="Email Address" />
      <Textarea placeholder="Tell us about yourself..." />
      <Button>Submit</Button>
    </div>
  </section>

  {/* Our Work */}
  <section id="work" className="py-16 px-8 max-w-5xl mx-auto">
    <h3 className="text-3xl font-semibold mb-6">Our Work</h3>
    <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
      <Card>
        <CardContent className="p-4">
          <h4 className="text-xl font-bold mb-2">Plastic-to-Fuel Project</h4>
          <p>Transforming plastic waste into sustainable energy for a cleaner Botswana.</p>
        </CardContent>
      </Card>
      <Card>
        <CardContent className="p-4">
          <h4 className="text-xl font-bold mb-2">Hydrogen Combustion Engine</h4>
          <p>A new leap into clean transport using alternative fuel innovations.</p>
        </CardContent>
      </Card>
    </div>
  </section>

  {/* Blog/Updates */}
  <section id="blog" className="py-16 px-8 bg-gray-50">
    <h3 className="text-3xl font-semibold mb-4">Blog & Updates</h3>
    <p>Coming soon: Stories, updates, and insights from our journey of innovation.</p>
  </section>

  {/* Contact */}
  <section id="contact" className="py-16 px-8 max-w-4xl mx-auto">
    <h3 className="text-3xl font-semibold mb-6">Contact Us</h3>
    <p className="mb-4">Get in touch with us on social platforms or drop a message:</p>
    <div className="flex space-x-4 mb-4">
      <a href="https://www.instagram.com/innovators_hub1" target="_blank" rel="noopener noreferrer"><Instagram /></a>
      <a href="https://tiktok.com/@innovators_hub3" target="_blank" rel="noopener noreferrer"><Tiktok /></a>
      <Mail /><span>mphophillimon6@gmail.com</span>
      <Phone /><span>+267 76020226 / 72695770</span>
    </div>
    <div className="space-y-4">
      <Input placeholder="Your Email" />
      <Textarea placeholder="Your Message" />
      <Button>Send</Button>
    </div>
  </section>

  {/* Footer */}
  <footer className="text-center p-4 bg-black text-white mt-10">
    &copy; {new Date().getFullYear()} Creative Innovation Group | Powered by MacPhill
  </footer>
</div>

); }

