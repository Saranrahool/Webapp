import React from "react";
import { BrowserRouter as Router, Route, Routes, Link } from "react-router-dom";
import { Button } from "@/components/ui/button";

const Home = () => {
  return (
    <div className="flex flex-col items-center justify-center h-screen">
      <h1 className="text-4xl font-bold mb-4">Welcome to My Website</h1>
      <p className="text-lg text-gray-600 mb-4">A simple web app using React and Tailwind CSS</p>
      <Button asChild>
        <Link to="/about">Learn More</Link>
      </Button>
    </div>
  );
};

const About = () => {
  return (
    <div className="flex flex-col items-center justify-center h-screen">
      <h1 className="text-3xl font-bold mb-4">About Us</h1>
      <p className="text-lg text-gray-600">This is a simple web app created with React.</p>
      <Button asChild>
        <Link to="/">Go Home</Link>
      </Button>
    </div>
  );
};

const Navbar = () => {
  return (
    <nav className="p-4 bg-gray-800 text-white flex justify-between">
      <h1 className="text-xl font-bold">My Website</h1>
      <div className="space-x-4">
        <Link to="/" className="hover:underline">Home</Link>
        <Link to="/about" className="hover:underline">About</Link>
      </div>
    </nav>
  );
};

const App = () => {
  return (
    <Router>
      <Navbar />
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/about" element={<About />} />
      </Routes>
    </Router>
  );
};

export default App;
