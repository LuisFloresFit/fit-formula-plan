import React from 'react';
import { Button } from '@/components/ui/button';

export default function FitFormula() {
  return (
    <div className="bg-black text-white min-h-screen p-6 space-y-10">
      {/* Hero Section */}
      <section className="text-center space-y-4">
        <h1 className="text-4xl font-bold">Fit Formula Plan: Your Total Wellness Transformation</h1>
        <p className="text-lg max-w-2xl mx-auto">
          Discover a science-backed approach to sustainable fitness and nutrition that adapts to your unique body and lifestyle.
        </p>
        <Button className="bg-green-500 hover:bg-green-600 text-white text-lg">Start Your Transformation</Button>
      </section>

      {/* How It Works Section */}
      <section>
        <h2 className="text-3xl font-bold mb-4 text-center">How Fit Formula Works</h2>
        <div className="grid md:grid-cols-3 gap-6 text-center">
          <div>
            <h3 className="text-xl font-semibold">Analyze</h3>
            <p>Complete a quick questionnaire to help us craft a personalized workout plan.</p>
          </div>
          <div>
            <h3 className="text-xl font-semibold">Nourish</h3>
            <p>Follow your custom meal plan with targeted macros and delicious recipes.</p>
          </div>
          <div>
            <h3 className="text-xl font-semibold">Train</h3>
            <p>Execute evolving workouts to maximize results and prevent plateaus.</p>
          </div>
        </div>
      </section>

      {/* Nutrition Strategy Section */}
      <section>
        <h2 className="text-3xl font-bold mb-4 text-center">Nutrition Strategy</h2>
        <div className="space-y-4">
          <p><strong>Macro-Balanced Meal Planning:</strong> Personalized protein, carb, and fat ratios.</p>
          <p><strong>Extensive Recipe Library:</strong> 500+ chef-developed recipes, including keto, paleo, vegan, and carb cycling.</p>
          <p><strong>Dynamic Calorie Targeting:</strong> Adjusts based on activity, intensity, and goals.</p>
          <p><strong>Dietary Flexibility:</strong> Accommodates gluten-free, dairy-free, and other protocols.</p>
        </div>
      </section>

      {/* Workout Blueprints Section */}
      <section>
        <h2 className="text-3xl font-bold mb-4 text-center">Workout Blueprints</h2>
        <div className="grid md:grid-cols-4 gap-4 text-center">
          {['Beginner', 'Intermediate', 'Advanced', 'Elite'].map(level => (
            <div key={level}>
              <h3 className="text-xl font-semibold">{level}</h3>
              <p>{
                level === 'Beginner' ? 'Foundation-building workouts focusing on proper form.' :
                level === 'Intermediate' ? 'Progressive circuits for muscle definition.' :
                level === 'Advanced' ? 'High-intensity training for fat loss and muscle growth.' :
                'Performance-focused training with advanced techniques.'
              }</p>
            </div>
          ))}
        </div>
        <p className="text-center mt-4">All workouts include home/gym modifications and progressive overload.</p>
      </section>

      {/* Success Stories Section */}
      <section>
        <h2 className="text-3xl font-bold mb-4 text-center">Success Stories</h2>
        <div className="grid md:grid-cols-2 gap-6">
          <div>
            <h3 className="text-xl font-semibold">Anyssa, 26</h3>
            <p>"I started off as a complete beginner... Now, 3 months in, I’m stronger, leaner, and more motivated than ever."</p>
          </div>
          <div>
            <h3 className="text-xl font-semibold">Luis, 25</h3>
            <p>"Real talk—results didn’t show up overnight... but the transformation has been worth every second!"</p>
          </div>
        </div>
      </section>

      {/* Pricing Section */}
      <section>
        <h2 className="text-3xl font-bold mb-4 text-center">Pricing & Plans</h2>
        <div className="max-w-xl mx-auto text-center space-y-2">
          <p><strong>Basic Workout Plan:</strong> $60 (One-Time)</p>
          <p><strong>Workout + Meal Plan:</strong> $70 (One-Time)</p>
          <p className="text-sm text-gray-400">*Update your plan every 3 months to avoid plateaus.*</p>
        </div>
      </section>

      {/* Getting Started Section */}
      <section className="text-center space-y-4">
        <h2 className="text-3xl font-bold">Getting Started</h2>
        <p><strong>Transform:</strong> Begin your journey to a healthier, stronger you.</p>
        <p><strong>Implement:</strong> Follow your personalized plan.</p>
        <p><strong>Analyze:</strong> Complete your comprehensive health assessment.</p>
        <Button className="bg-green-500 hover:bg-green-600 text-white text-lg">Join Now</Button>
      </section>
    </div>
  );
}
