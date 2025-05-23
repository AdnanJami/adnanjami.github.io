import React from 'react';
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Github, Linkedin } from "lucide-react";

export default function Portfolio() {
  return (
    <div className="min-h-screen bg-gray-100 p-6">
      <div className="max-w-4xl mx-auto space-y-6">
        <header className="text-center">
          <h1 className="text-4xl font-bold">Abdullah Mohammad Muntasir Adnan Jami</h1>
          <p className="text-lg text-gray-600 mt-2">CSE Undergraduate | Robotics & AI Enthusiast | Generative AI Explorer</p>
          <div className="mt-4 flex justify-center space-x-4">
            <a href="https://github.com/AdnanJami" target="_blank" rel="noopener noreferrer">
              <Button variant="outline"><Github className="mr-2" /> GitHub</Button>
            </a>
            <a href="https://www.linkedin.com/in/adnan-jami-27795823b/" target="_blank" rel="noopener noreferrer">
              <Button variant="outline"><Linkedin className="mr-2" /> LinkedIn</Button>
            </a>
          </div>
        </header>

        <section>
          <h2 className="text-2xl font-semibold mb-2">About Me</h2>
          <Card>
            <CardContent className="p-4 text-gray-700">
              I'm a passionate CSE undergraduate from North South University, deeply interested in AI, robotics, and cybersecurity. I've built autonomous robots, participated in international competitions, and I'm currently working on a research paper in generative AI.
            </CardContent>
          </Card>
        </section>

        <section>
          <h2 className="text-2xl font-semibold mb-2">Projects</h2>
          <div className="grid gap-4 md:grid-cols-2">
            <Card>
              <CardContent className="p-4">
                <h3 className="font-bold">AI-Controlled Robot</h3>
                <p className="text-gray-700">Autonomous robot using sensors and AI-based decision-making, with real-time object detection.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent className="p-4">
                <h3 className="font-bold">POS Software</h3>
                <p className="text-gray-700">A fully functional point-of-sale system built using PHP and SQL for inventory and transaction management.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent className="p-4">
                <h3 className="font-bold">Object Detection System</h3>
                <p className="text-gray-700">Implemented object recognition models to classify and identify real-world objects using Python.</p>
              </CardContent>
            </Card>
          </div>
        </section>

        <section>
          <h2 className="text-2xl font-semibold mb-2">Skills</h2>
          <Card>
            <CardContent className="p-4 text-gray-700">
              <ul className="list-disc list-inside">
                <li>C, Python, SQL, PHP</li>
                <li>Generative AI, Object Detection, Robotics</li>
                <li>Google Colab, Kaggle, Git</li>
                <li>Basic Networking, Cybersecurity Interest</li>
              </ul>
            </CardContent>
          </Card>
        </section>

        <section>
          <h2 className="text-2xl font-semibold mb-2">Achievements</h2>
          <Card>
            <CardContent className="p-4 text-gray-700">
              <ul className="list-disc list-inside">
                <li>Co-authoring a research paper on Generative AI</li>
                <li>Participant in ICPC, KIBO Robot Programming Challenge</li>
                <li>CTF cybersecurity competition experience</li>
              </ul>
            </CardContent>
          </Card>
        </section>
      </div>
    </div>
  );
}
