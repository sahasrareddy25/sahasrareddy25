import React from "react";
import { Github, Linkedin, Mail, Code, Trophy } from "lucide-react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";

export default function GitHubResume() {
  return (
    <div className="min-h-screen bg-slate-950 text-slate-100 px-6 py-10">
      <div className="max-w-5xl mx-auto space-y-10">

        {/* Header */}
        <section className="text-center space-y-4">
          <h1 className="text-4xl font-bold tracking-tight">Sahasra Reddy</h1>
          <p className="text-slate-400 text-lg">
            B.Tech CSE | Aspiring Product-Based Software Engineer
          </p>
          <div className="flex justify-center gap-4">
            <Button variant="outline" className="rounded-2xl">
              <Github className="mr-2 h-4 w-4" /> GitHub
            </Button>
            <Button variant="outline" className="rounded-2xl">
              <Linkedin className="mr-2 h-4 w-4" /> LinkedIn
            </Button>
            <Button variant="outline" className="rounded-2xl">
              <Mail className="mr-2 h-4 w-4" /> Email
            </Button>
          </div>
        </section>

        {/* About */}
        <Card className="rounded-2xl shadow-lg">
          <CardContent className="p-6 space-y-3">
            <h2 className="text-xl font-semibold">About Me</h2>
            <p className="text-slate-300 leading-relaxed">
              I am a 3rd-year Computer Science Engineering student at Mallareddy University,
              actively preparing for product-based company roles. I focus on building strong
              fundamentals in Data Structures, Algorithms, Python, and Full-Stack Development.
              I enjoy solving real-world problems and converting ideas into scalable solutions.
            </p>
          </CardContent>
        </Card>

        {/* Skills */}
        <Card className="rounded-2xl">
          <CardContent className="p-6">
            <h2 className="text-xl font-semibold mb-4">Skills</h2>
            <div className="grid grid-cols-2 md:grid-cols-4 gap-4">
              {["Python", "JavaScript", "React", "Flask", "SQL", "DSA", "Git & GitHub", "APIs"].map(
                (skill) => (
                  <div
                    key={skill}
                    className="bg-slate-900 border border-slate-800 rounded-xl py-2 text-center"
                  >
                    {skill}
                  </div>
                )
              )}
            </div>
          </CardContent>
        </Card>

        {/* Projects */}
        <Card className="rounded-2xl">
          <CardContent className="p-6 space-y-4">
            <h2 className="text-xl font-semibold">Projects</h2>
            <ul className="space-y-3">
              <li>
                <strong>JANSEVA LINK</strong> – AI-Assisted Citizen Grievance Platform using Flask & SQLite
              </li>
              <li>
                <strong>Ola Ride Demand Forecast</strong> – Streamlit-based ML prediction app
              </li>
              <li>
                <strong>Smart Shelf</strong> – IoT-based food spoilage detection system
              </li>
            </ul>
          </CardContent>
        </Card>

        {/* Achievements */}
        <Card className="rounded-2xl">
          <CardContent className="p-6">
            <h2 className="text-xl font-semibold mb-3">Achievements</h2>
            <p className="flex items-center gap-2">
              <Trophy className="h-4 w-4 text-yellow-400" /> Solved 25+ LeetCode problems
            </p>
          </CardContent>
        </Card>

        {/* Footer */}
        <footer className="text-center text-slate-500 text-sm">
          Built with React • Designed for GitHub Resume & Interviews
        </footer>
      </div>
    </div>
  );
}

