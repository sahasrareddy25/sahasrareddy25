# 👋 Hi, I'm Sahasra Reddy Perati
# 🎓 B.Tech CSE | 3rd Year | Mallareddy University
# 💡 Aspiring Product-Based Software Engineer

class Developer:
    def __init__(self):
        self.name = "Sahasra Reddy"
        self.role = "CSE Undergraduate"
        self.location = "Hyderabad, India"
        
        self.core_language = "Python 🐍"
        self.learning_stack = [
            "Data Structures & Algorithms",
            "Problem Solving (LeetCode)",
            "APIs & Backend Basics",
            "AI / Computer Vision"
        ]
        
        self.projects = {
            "Ola Ride Forecast": "Demand prediction using ML & Streamlit",
            "Cartoonizer": "Image processing with OpenCV",
            "JANSEVA LINK": "AI-assisted citizen grievance platform (Hackathon)"
        }
        
        self.mindset = {
            "curiosity": "always learning",
            "consistency": "daily practice",
            "goal": "product-based company placement"
        }

    def daily_routine(self):
        return [
            "Solve LeetCode problems 🧩",
            "Build small but real projects 🛠️",
            "Learn concepts from basics 📘",
            "Improve one skill every day 📈"
        ]

    def future(self):
        return "Turning logic into impact — one commit at a time 🚀"


me = Developer()

print(me.future())
