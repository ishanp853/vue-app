<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <div>
    <section class="hero" id="hero">
      <video autoplay muted loop playsinline class="hero-video">
        <source src="https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4" type="video/mp4">
      </video>
      <div class="hero-overlay"></div>
      <div class="hero-content">
        <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=200&h=200&fit=crop" alt="Logo" class="hero-logo">
        <h1 class="hero-headline">Transform Your Business with AI-Powered Solutions</h1>
        <p class="hero-subheadline">Scale 10x faster, reduce costs by 60%, and revolutionize your workflow. Join 50,000+ companies already transforming their operations.</p>
        <button class="cta-button primary large" @click="scrollTo('features')">Start Free Trial</button>
        <div class="hero-badges">
          <img src="https://images.unsplash.com/photo-1611162617474-5b21e879e113?w=150&h=80&fit=crop" alt="Award" class="badge-img">
          <img src="https://images.unsplash.com/photo-1611162616305-c69b3fa7fbe0?w=150&h=80&fit=crop" alt="Certified" class="badge-img">
          <img src="https://images.unsplash.com/photo-1611162618071-b39a75ecbdf9?w=150&h=80&fit=crop" alt="Trusted" class="badge-img">
        </div>
      </div>
    </section>

    <section class="image-section left" id="features">
      <div class="container">
        <div class="image-content">
          <span class="section-badge">Powerful Features</span>
          <h2>Everything You Need to Succeed</h2>
          <p>Our platform combines cutting-edge technology with intuitive design, making complex automation accessible to everyone.</p>
          <ul class="feature-list">
            <li><img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?w=40&h=40&fit=crop" alt="Icon" class="list-icon"> Visual workflow builder</li>
            <li><img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=40&h=40&fit=crop" alt="Icon" class="list-icon"> Real-time analytics</li>
            <li><img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?w=40&h=40&fit=crop" alt="Icon" class="list-icon"> Enterprise security</li>
            <li><img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=40&h=40&fit=crop" alt="Icon" class="list-icon"> 500+ integrations</li>
          </ul>
          <button class="cta-button secondary" @click="scrollTo('use-cases')">Explore Features</button>
        </div>
        <div class="image-placeholder">
          <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?w=800&h=600&fit=crop" alt="Dashboard" class="section-image">
        </div>
      </div>
    </section>

    <section class="image-section right">
      <div class="container">
        <div class="image-placeholder">
          <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=800&h=600&fit=crop" alt="Analytics" class="section-image">
        </div>
        <div class="image-content">
          <span class="section-badge">Real-Time Insights</span>
          <h2>Make Data-Driven Decisions</h2>
          <p>Transform raw data into actionable insights with our comprehensive analytics platform.</p>
          <div class="image-grid-small">
            <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=200&h=150&fit=crop" alt="Chart 1" class="small-image">
            <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?w=200&h=150&fit=crop" alt="Chart 2" class="small-image">
            <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?w=200&h=150&fit=crop" alt="Chart 3" class="small-image">
            <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=200&h=150&fit=crop" alt="Chart 4" class="small-image">
          </div>
          <button class="cta-button secondary" @click="scrollTo('pricing')">View Analytics</button>
        </div>
      </div>
    </section>

    <section class="image-section left">
      <div class="container">
        <div class="image-content">
          <span class="section-badge">Seamless Integration</span>
          <h2>Connect All Your Tools</h2>
          <p>Integrate with your existing tech stack effortlessly. From CRM to marketing platforms.</p>
          <div class="integration-logos">
            <img src="https://images.unsplash.com/photo-1611162617474-5b21e879e113?w=120&h=120&fit=crop" alt="Integration 1" class="logo-img">
            <img src="https://images.unsplash.com/photo-1611162616305-c69b3fa7fbe0?w=120&h=120&fit=crop" alt="Integration 2" class="logo-img">
            <img src="https://images.unsplash.com/photo-1611162618071-b39a75ecbdf9?w=120&h=120&fit=crop" alt="Integration 3" class="logo-img">
            <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?w=120&h=120&fit=crop" alt="Integration 4" class="logo-img">
            <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=120&h=120&fit=crop" alt="Integration 5" class="logo-img">
            <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?w=120&h=120&fit=crop" alt="Integration 6" class="logo-img">
          </div>
          <button class="cta-button secondary" @click="scrollTo('integrations')">See All Integrations</button>
        </div>
        <div class="image-placeholder">
          <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?w=800&h=600&fit=crop" alt="Integrations" class="section-image">
        </div>
      </div>
    </section>

    <section class="features-grid-section">
      <div class="container">
        <div class="section-header">
          <span class="section-badge">Features</span>
          <h2>Powerful Features for Every Team</h2>
          <p class="section-subtitle">Everything you need to automate, analyze, and accelerate your business.</p>
        </div>
        <div class="features-grid">
          <div class="feature-card" v-for="(feature, index) in features" :key="index">
            <img :src="feature.image" :alt="feature.title" class="feature-icon">
            <h3>{{ feature.title }}</h3>
            <p>{{ feature.description }}</p>
            <img :src="feature.screenshot" :alt="feature.title + ' Screenshot'" class="feature-screenshot">
          </div>
        </div>
      </div>
    </section>

    <section class="long-content" id="use-cases">
      <div class="container">
        <div class="content-header">
          <span class="section-badge">Use Cases</span>
          <h2>How Industry Leaders Transform Operations</h2>
          <p class="section-intro">Discover how companies across industries leverage our platform to achieve remarkable results.</p>
        </div>

        <div class="content-grid">
          <div class="content-block" v-for="(useCase, index) in useCases" :key="index">
            <img :src="useCase.image" :alt="useCase.title" class="content-image">
            <div class="content-icon">📧</div>
            <h3>{{ useCase.title }}</h3>
            <p>{{ useCase.description }}</p>
            <ul>
              <li v-for="(item, i) in useCase.items" :key="i">{{ item }}</li>
            </ul>
            <div class="content-metrics">
              <div class="metric" v-for="(metric, m) in useCase.metrics" :key="m">{{ metric }}</div>
            </div>
          </div>
        </div>

        <div class="detailed-features">
          <h3>Enterprise-Grade Technical Capabilities</h3>
          <p class="features-intro">Built for scale, security, and reliability. Our platform handles millions of operations daily.</p>
          <div class="feature-grid">
            <div class="feature-item" v-for="(tech, index) in technicalFeatures" :key="index">
              <img :src="tech.image" :alt="tech.title" class="tech-icon">
              <h4>{{ tech.title }}</h4>
              <p>{{ tech.description }}</p>
              <ul class="feature-sublist">
                <li v-for="(item, i) in tech.items" :key="i">{{ item }}</li>
              </ul>
            </div>
          </div>
        </div>

        <div class="industry-solutions">
          <h3>Tailored Solutions for Every Industry</h3>
          <div class="industry-grid">
            <div class="industry-card" v-for="(industry, index) in industries" :key="index">
              <img :src="industry.image" :alt="industry.name" class="industry-image">
              <div class="industry-icon">{{ industry.icon }}</div>
              <h4>{{ industry.name }}</h4>
              <p>{{ industry.description }}</p>
            </div>
          </div>
        </div>

        <div class="benefits-section">
          <h3>Why Thousands of Teams Choose Us</h3>
          <div class="benefits-grid">
            <div class="benefit-item" v-for="(benefit, index) in benefits" :key="index">
              <img :src="benefit.image" :alt="benefit.title" class="benefit-image">
              <div class="benefit-number">{{ String(index + 1).padStart(2, '0') }}</div>
              <h4>{{ benefit.title }}</h4>
              <p>{{ benefit.description }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="testimonials">
      <div class="container">
        <div class="section-header">
          <span class="section-badge">Testimonials</span>
          <h2>Trusted by Industry Leaders Worldwide</h2>
          <p class="section-subtitle">See what our customers have to say about their experience.</p>
        </div>
        <div class="testimonial-grid">
          <div class="testimonial-card" v-for="(testimonial, index) in testimonials" :key="index">
            <img :src="testimonial.starsImage" alt="Stars" class="stars-image">
            <p class="testimonial-text">"{{ testimonial.text }}"</p>
            <div class="author">
              <img :src="testimonial.avatar" :alt="testimonial.name" class="avatar">
              <div class="author-info">
                <div class="author-name">{{ testimonial.name }}</div>
                <div class="author-title">{{ testimonial.title }}</div>
              </div>
            </div>
            <img :src="testimonial.companyLogo" alt="Company Logo" class="company-logo">
          </div>
        </div>
      </div>
    </section>

    <section class="pricing-section" id="pricing">
      <div class="container">
        <div class="section-header">
          <span class="section-badge">Pricing</span>
          <h2>Choose the Perfect Plan for Your Team</h2>
          <p class="section-subtitle">All plans include 24/7 support, daily backups, and 99.99% uptime guarantee.</p>
        </div>
        <div class="pricing-cards">
          <div class="pricing-card" v-for="(plan, index) in pricingPlans" :key="index" :class="{ popular: plan.popular }">
            <div class="popular-badge" v-if="plan.popular">Most Popular</div>
            <img :src="plan.image" :alt="plan.name" class="plan-image">
            <h3>{{ plan.name }}</h3>
            <div class="price">${{ plan.price }}<span>/month</span></div>
            <p class="price-description">{{ plan.description }}</p>
            <ul>
              <li v-for="(feature, f) in plan.features" :key="f">✓ {{ feature }}</li>
            </ul>
            <button class="cta-button" :class="{ primary: plan.popular }" @click="scrollTo('contact')">{{ plan.buttonText }}</button>
            <p class="trial-info">{{ plan.trialInfo }}</p>
          </div>
        </div>
        <div class="pricing-footer">
          <img src="https://images.unsplash.com/photo-1611162617474-5b21e879e113?w=400&h=100&fit=crop" alt="Security Badges" class="security-badges">
          <p>All plans include: Free onboarding, comprehensive documentation, community access, and regular feature updates.</p>
        </div>
      </div>
    </section>

    <section class="team-section">
      <div class="container">
        <div class="section-header">
          <span class="section-badge">Our Team</span>
          <h2>Meet the Experts Behind the Platform</h2>
          <p class="section-subtitle">A talented team dedicated to your success.</p>
        </div>
        <div class="team-grid">
          <div class="team-card" v-for="(member, index) in teamMembers" :key="index">
            <img :src="member.photo" :alt="member.name" class="team-photo">
            <h3>{{ member.name }}</h3>
            <div class="team-title">{{ member.title }}</div>
            <p>{{ member.bio }}</p>
            <div class="team-social">
              <img src="https://images.unsplash.com/photo-1611162617474-5b21e879e113?w=30&h=30&fit=crop" alt="LinkedIn" class="social-icon">
              <img src="https://images.unsplash.com/photo-1611162616305-c69b3fa7fbe0?w=30&h=30&fit=crop" alt="Twitter" class="social-icon">
              <img src="https://images.unsplash.com/photo-1611162618071-b39a75ecbdf9?w=30&h=30&fit=crop" alt="GitHub" class="social-icon">
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="cta-section" id="demo">
      <div class="container">
        <div class="cta-content">
          <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?w=600&h=400&fit=crop" alt="Demo" class="cta-image">
          <div class="cta-text">
            <h2>See It In Action</h2>
            <p>Watch a 5-minute demo and see how our platform can transform your business operations.</p>
            <div class="cta-buttons">
              <button class="cta-button primary large" @click="scrollTo('contact')">Watch Demo</button>
              <button class="cta-button secondary large" @click="scrollTo('pricing')">View Pricing</button>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="cta-section-alt">
      <div class="container">
        <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=800&h=500&fit=crop" alt="CTA Background" class="cta-bg-image">
        <div class="cta-overlay-content">
          <h2>Ready to Get Started?</h2>
          <p>Join thousands of companies already using our platform</p>
          <button class="cta-button primary large" @click="scrollTo('contact')">Start Free Trial</button>
        </div>
      </div>
    </section>

    <section class="final-cta" id="contact">
      <div class="container">
        <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?w=200&h=200&fit=crop" alt="Logo" class="final-logo">
        <h2>Ready to Transform Your Business?</h2>
        <p class="cta-subtitle">Join 50,000+ teams already automating their success. Start your free trial today.</p>
        <div class="cta-buttons">
          <button class="cta-button primary large" @click="scrollTo('hero')">Start Free Trial</button>
          <button class="cta-button secondary large">Schedule Demo</button>
          <button class="cta-button secondary large">Contact Sales</button>
        </div>
        <div class="cta-features">
          <div class="cta-feature">✓ 14-day free trial</div>
          <div class="cta-feature">✓ No credit card required</div>
          <div class="cta-feature">✓ Cancel anytime</div>
          <div class="cta-feature">✓ Full feature access</div>
        </div>
        <div class="trust-logos">
          <img src="https://images.unsplash.com/photo-1611162617474-5b21e879e113?w=150&h=80&fit=crop" alt="Trust Logo 1" class="trust-logo">
          <img src="https://images.unsplash.com/photo-1611162616305-c69b3fa7fbe0?w=150&h=80&fit=crop" alt="Trust Logo 2" class="trust-logo">
          <img src="https://images.unsplash.com/photo-1611162618071-b39a75ecbdf9?w=150&h=80&fit=crop" alt="Trust Logo 3" class="trust-logo">
          <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?w=150&h=80&fit=crop" alt="Trust Logo 4" class="trust-logo">
        </div>
      </div>
    </section>

    <footer class="footer">
      <div class="container">
        <div class="footer-top">
          <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=200&h=80&fit=crop" alt="Logo" class="footer-logo">
          <p class="footer-tagline">Transform your business with AI-powered automation</p>
        </div>
        <div class="footer-content">
          <div class="footer-section">
            <h4>Product</h4>
            <ul>
              <li><a href="#features">Features</a></li>
              <li><a href="#pricing">Pricing</a></li>
              <li><a href="#integrations">Integrations</a></li>
              <li><a href="#">Security</a></li>
              <li><a href="#">API Documentation</a></li>
            </ul>
          </div>
          <div class="footer-section">
            <h4>Company</h4>
            <ul>
              <li><a href="#">About Us</a></li>
              <li><a href="#">Careers</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">Press Kit</a></li>
              <li><a href="#">Contact</a></li>
            </ul>
          </div>
          <div class="footer-section">
            <h4>Resources</h4>
            <ul>
              <li><a href="#">Documentation</a></li>
              <li><a href="#">Help Center</a></li>
              <li><a href="#">Community</a></li>
              <li><a href="#">Webinars</a></li>
              <li><a href="#">Case Studies</a></li>
            </ul>
          </div>
          <div class="footer-section">
            <h4>Legal</h4>
            <ul>
              <li><a href="#">Privacy Policy</a></li>
              <li><a href="#">Terms of Service</a></li>
              <li><a href="#">Cookie Policy</a></li>
              <li><a href="#">GDPR Compliance</a></li>
            </ul>
          </div>
        </div>
        <div class="footer-bottom">
          <p>&copy; 2024 AI Automation Platform. All rights reserved.</p>
          <div class="footer-social">
            <img src="https://images.unsplash.com/photo-1611162617474-5b21e879e113?w=40&h=40&fit=crop" alt="LinkedIn" class="social-icon-img">
            <img src="https://images.unsplash.com/photo-1611162616305-c69b3fa7fbe0?w=40&h=40&fit=crop" alt="Twitter" class="social-icon-img">
            <img src="https://images.unsplash.com/photo-1611162618071-b39a75ecbdf9?w=40&h=40&fit=crop" alt="Facebook" class="social-icon-img">
            <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?w=40&h=40&fit=crop" alt="YouTube" class="social-icon-img">
            <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=40&h=40&fit=crop" alt="Instagram" class="social-icon-img">
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  line-height: 1.6;
  color: #333;
  overflow-x: hidden;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.hero {
  position: relative;
  height: 100vh;
  min-height: 600px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: white;
  overflow: hidden;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}

.hero-video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: 1;
}

.hero-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(135deg, rgba(102, 126, 234, 0.85) 0%, rgba(118, 75, 162, 0.85) 100%);
  z-index: 2;
}

.hero-content {
  position: relative;
  z-index: 3;
  max-width: 900px;
  padding: 0 20px;
}

.hero-logo {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  margin-bottom: 2rem;
  border: 4px solid rgba(255,255,255,0.3);
  box-shadow: 0 10px 40px rgba(0,0,0,0.3);
}

.hero-headline {
  font-size: clamp(2.5rem, 6vw, 4.5rem);
  font-weight: 800;
  margin-bottom: 1.5rem;
  line-height: 1.1;
  text-shadow: 0 2px 20px rgba(0,0,0,0.3);
}

.hero-subheadline {
  font-size: clamp(1.1rem, 2.5vw, 1.5rem);
  margin-bottom: 2.5rem;
  opacity: 0.95;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
  line-height: 1.6;
}

.hero-badges {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin-top: 3rem;
  flex-wrap: wrap;
}

.badge-img {
  height: 60px;
  width: auto;
  opacity: 0.9;
  border-radius: 8px;
}

.cta-button {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  border: none;
  padding: 1rem 2.5rem;
  font-size: 1.1rem;
  font-weight: 600;
  border-radius: 50px;
  cursor: pointer;
  transition: all 0.3s ease;
  font-family: inherit;
}

.cta-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 20px 40px rgba(0,0,0,0.3);
}

.cta-button.primary {
  background: linear-gradient(135deg, #ff6b6b 0%, #feca57 100%);
}

.cta-button.primary:hover {
  box-shadow: 0 20px 40px rgba(255, 107, 107, 0.4);
}

.cta-button.secondary {
  background: transparent;
  border: 2px solid white;
  color: white;
}

.cta-button.secondary:hover {
  background: rgba(255,255,255,0.1);
}

.cta-button.large {
  padding: 1.5rem 3.5rem;
  font-size: 1.3rem;
}

.image-section {
  padding: 120px 0;
  background: white;
}

.image-section:nth-child(even) {
  background: #f8fafc;
}

.image-section .container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 4rem;
  align-items: center;
}

.image-section.right .container {
  direction: rtl;
}

.image-section.right .image-content {
  direction: ltr;
}

.section-badge {
  display: inline-block;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 0.5rem 1.5rem;
  border-radius: 50px;
  font-size: 0.85rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 1px;
  margin-bottom: 1.5rem;
}

.image-content h2 {
  font-size: clamp(2rem, 4vw, 3rem);
  font-weight: 700;
  margin-bottom: 1.5rem;
  color: #1e293b;
  line-height: 1.2;
}

.image-content > p {
  font-size: 1.2rem;
  margin-bottom: 2rem;
  color: #64748b;
  line-height: 1.7;
}

.feature-list {
  list-style: none;
  margin-bottom: 2.5rem;
}

.feature-list li {
  font-size: 1.1rem;
  padding: 0.75rem 0;
  color: #475569;
  display: flex;
  align-items: center;
  gap: 1rem;
}

.list-icon {
  width: 40px;
  height: 40px;
  border-radius: 8px;
  flex-shrink: 0;
}

.section-image {
  width: 100%;
  height: auto;
  border-radius: 20px;
  box-shadow: 0 30px 60px rgba(0,0,0,0.15);
}

.image-grid-small {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1rem;
  margin-bottom: 2rem;
}

.small-image {
  width: 100%;
  height: 150px;
  object-fit: cover;
  border-radius: 12px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
}

.integration-logos {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.5rem;
  margin-bottom: 2rem;
}

.logo-img {
  width: 100%;
  height: 120px;
  object-fit: cover;
  border-radius: 12px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}

.features-grid-section {
  padding: 120px 0;
  background: #f8fafc;
}

.section-header {
  text-align: center;
  margin-bottom: 4rem;
}

.section-header h2 {
  font-size: clamp(2.5rem, 5vw, 3.5rem);
  margin: 1.5rem 0;
  color: #1e293b;
}

.section-subtitle {
  font-size: 1.2rem;
  color: #64748b;
  max-width: 700px;
  margin: 0 auto;
  line-height: 1.7;
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2.5rem;
}

.feature-card {
  background: white;
  padding: 2.5rem;
  border-radius: 20px;
  box-shadow: 0 10px 40px rgba(0,0,0,0.08);
  text-align: center;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.feature-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 20px 60px rgba(0,0,0,0.15);
}

.feature-icon {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  margin-bottom: 1.5rem;
  border: 4px solid #f1f5f9;
}

.feature-card h3 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #1e293b;
}

.feature-card p {
  color: #64748b;
  margin-bottom: 1.5rem;
  line-height: 1.7;
}

.feature-screenshot {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 12px;
  margin-top: 1.5rem;
}

.long-content {
  padding: 120px 0;
  background: white;
}

.content-header {
  text-align: center;
  margin-bottom: 4rem;
}

.content-header h2 {
  font-size: clamp(2.5rem, 5vw, 3.5rem);
  margin: 1.5rem 0;
  color: #1e293b;
}

.section-intro {
  font-size: 1.3rem;
  color: #64748b;
  max-width: 800px;
  margin: 0 auto;
  line-height: 1.7;
}

.content-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(500px, 1fr));
  gap: 3rem;
  margin-bottom: 6rem;
}

.content-block {
  background: white;
  padding: 3rem;
  border-radius: 20px;
  box-shadow: 0 10px 40px rgba(0,0,0,0.08);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.content-block:hover {
  transform: translateY(-5px);
  box-shadow: 0 20px 60px rgba(0,0,0,0.12);
}

.content-image {
  width: 100%;
  height: 300px;
  object-fit: cover;
  border-radius: 15px;
  margin-bottom: 2rem;
}

.content-icon {
  font-size: 3rem;
  margin-bottom: 1.5rem;
}

.content-block h3 {
  font-size: 1.8rem;
  margin-bottom: 1.5rem;
  color: #1e293b;
}

.content-block > p {
  color: #64748b;
  margin-bottom: 1.5rem;
  font-size: 1.1rem;
  line-height: 1.7;
}

.content-block ul {
  list-style: none;
  margin-bottom: 2rem;
}

.content-block li {
  padding: 0.75rem 0;
  color: #475569;
  line-height: 1.6;
  padding-left: 1.5rem;
  position: relative;
}

.content-block li:before {
  content: '→';
  position: absolute;
  left: 0;
  color: #667eea;
  font-weight: bold;
}

.content-metrics {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
  margin-top: 2rem;
  padding-top: 2rem;
  border-top: 2px solid #f1f5f9;
}

.metric {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 0.75rem 1.5rem;
  border-radius: 50px;
  font-weight: 600;
  font-size: 0.9rem;
}

.detailed-features {
  background: white;
  padding: 4rem;
  border-radius: 20px;
  box-shadow: 0 20px 60px rgba(0,0,0,0.1);
  margin-bottom: 4rem;
}

.detailed-features h3 {
  text-align: center;
  font-size: 2.5rem;
  margin-bottom: 1rem;
  color: #1e293b;
}

.features-intro {
  text-align: center;
  font-size: 1.2rem;
  color: #64748b;
  margin-bottom: 3rem;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
}

.feature-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2.5rem;
  margin-top: 3rem;
}

.feature-item {
  padding: 2rem;
  border-radius: 15px;
  background: #f8fafc;
  transition: transform 0.3s ease;
  text-align: center;
}

.feature-item:hover {
  transform: translateY(-5px);
  background: white;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
}

.tech-icon {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  margin-bottom: 1.5rem;
  border: 4px solid #e2e8f0;
}

.feature-item h4 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #1e293b;
}

.feature-item > p {
  color: #64748b;
  margin-bottom: 1.5rem;
  line-height: 1.7;
}

.feature-sublist {
  list-style: none;
  text-align: left;
}

.feature-sublist li {
  padding: 0.5rem 0;
  color: #475569;
  padding-left: 1.5rem;
  position: relative;
}

.feature-sublist li:before {
  content: '•';
  position: absolute;
  left: 0;
  color: #667eea;
  font-weight: bold;
  font-size: 1.2rem;
}

.industry-solutions {
  background: white;
  padding: 4rem;
  border-radius: 20px;
  box-shadow: 0 20px 60px rgba(0,0,0,0.1);
  margin-bottom: 4rem;
}


<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  line-height: 1.6;
  color: #333;
  overflow-x: hidden;
}

#app {
  min-height: 100vh;
  overflow-x: hidden;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

/* Hero Section */
.hero {
  position: relative;
  height: 100vh;
  min-height: 600px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: white;
  overflow: hidden;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}

.hero-video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: 1;
}

.hero-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(135deg, rgba(102, 126, 234, 0.85) 0%, rgba(118, 75, 162, 0.85) 100%);
  z-index: 2;
}

.hero-content {
  position: relative;
  z-index: 3;
  max-width: 900px;
  padding: 0 20px;
}

.hero-headline {
  font-size: clamp(2.5rem, 6vw, 4.5rem);
  font-weight: 800;
  margin-bottom: 1.5rem;
  line-height: 1.1;
  text-shadow: 0 2px 20px rgba(0,0,0,0.3);
}

.hero-subheadline {
  font-size: clamp(1.1rem, 2.5vw, 1.5rem);
  margin-bottom: 2.5rem;
  opacity: 0.95;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
  line-height: 1.6;
}

.hero-cta {
  display: flex;
  gap: 1.5rem;
  justify-content: center;
  flex-wrap: wrap;
  margin-bottom: 4rem;
}

.hero-stats {
  display: flex;
  justify-content: center;
  gap: 4rem;
  flex-wrap: wrap;
  margin-top: 3rem;
}

.stat-item {
  text-align: center;
}

.stat-number {
  font-size: 2.5rem;
  font-weight: 800;
  margin-bottom: 0.5rem;
}

.stat-label {
  font-size: 0.9rem;
  opacity: 0.9;
  text-transform: uppercase;
  letter-spacing: 1px;
}

/* CTA Buttons */
.cta-button {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  border: none;
  padding: 1rem 2.5rem;
  font-size: 1.1rem;
  font-weight: 600;
  border-radius: 50px;
  cursor: pointer;
  transition: all 0.3s ease;
  text-decoration: none;
  display: inline-block;
  font-family: inherit;
}

.cta-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 20px 40px rgba(0,0,0,0.3);
}

.cta-button:active {
  transform: translateY(0);
}

.cta-button.primary {
  background: linear-gradient(135deg, #ff6b6b 0%, #feca57 100%);
}

.cta-button.primary:hover {
  box-shadow: 0 20px 40px rgba(255, 107, 107, 0.4);
}

.cta-button.secondary {
  background: transparent;
  border: 2px solid white;
  color: white;
}

.cta-button.secondary:hover {
  background: rgba(255,255,255,0.1);
}

.cta-button.large {
  padding: 1.5rem 3.5rem;
  font-size: 1.3rem;
}

/* Image Sections */
.image-section {
  padding: 120px 0;
  background: white;
}

.image-section:nth-child(even) {
  background: #f8fafc;
}

.image-section .container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 4rem;
  align-items: center;
}

.image-section.right .container {
  direction: rtl;
}

.image-section.right .image-content {
  direction: ltr;
}

.section-badge {
  display: inline-block;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 0.5rem 1.5rem;
  border-radius: 50px;
  font-size: 0.85rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 1px;
  margin-bottom: 1.5rem;
}

.image-content h2 {
  font-size: clamp(2rem, 4vw, 3rem);
  font-weight: 700;
  margin-bottom: 1.5rem;
  color: #1e293b;
  line-height: 1.2;
}

.image-content > p {
  font-size: 1.2rem;
  margin-bottom: 2rem;
  color: #64748b;
  line-height: 1.7;
}

.feature-list {
  list-style: none;
  margin-bottom: 2.5rem;
}

.feature-list li {
  font-size: 1.1rem;
  padding: 0.75rem 0;
  color: #475569;
  display: flex;
  align-items: flex-start;
}

.image-placeholder {
  display: flex;
  justify-content: center;
  align-items: center;
}

.placeholder-image {
  width: 100%;
  height: 450px;
  border-radius: 20px;
  position: relative;
  box-shadow: 0 30px 60px rgba(0,0,0,0.15);
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

.feature-image {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}

.dashboard-image {
  background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
}

.integration-image {
  background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
}

.image-overlay-text {
  color: white;
  font-size: 2rem;
  font-weight: 700;
  text-shadow: 0 2px 10px rgba(0,0,0,0.2);
}

/* Long Content Section */
.long-content {
  padding: 120px 0;
  background: #f8fafc;
}

.content-header {
  text-align: center;
  margin-bottom: 4rem;
}

.content-header h2 {
  font-size: clamp(2.5rem, 5vw, 3.5rem);
  margin: 1.5rem 0;
  color: #1e293b;
}

.section-intro {
  font-size: 1.3rem;
  color: #64748b;
  max-width: 800px;
  margin: 0 auto;
  line-height: 1.7;
}

.content-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(500px, 1fr));
  gap: 3rem;
  margin-bottom: 6rem;
}

.content-block {
  background: white;
  padding: 3rem;
  border-radius: 20px;
  box-shadow: 0 10px 40px rgba(0,0,0,0.08);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.content-block:hover {
  transform: translateY(-5px);
  box-shadow: 0 20px 60px rgba(0,0,0,0.12);
}

.content-icon {
  font-size: 3rem;
  margin-bottom: 1.5rem;
}

.content-block h3 {
  font-size: 1.8rem;
  margin-bottom: 1.5rem;
  color: #1e293b;
}

.content-block > p {
  color: #64748b;
  margin-bottom: 1.5rem;
  font-size: 1.1rem;
  line-height: 1.7;
}

.content-block ul {
  list-style: none;
  margin-bottom: 2rem;
}

.content-block li {
  padding: 0.75rem 0;
  color: #475569;
  line-height: 1.6;
  padding-left: 1.5rem;
  position: relative;
}

.content-block li:before {
  content: '→';
  position: absolute;
  left: 0;
  color: #667eea;
  font-weight: bold;
}

.content-metrics {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
  margin-top: 2rem;
  padding-top: 2rem;
  border-top: 2px solid #f1f5f9;
}

.metric {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 0.75rem 1.5rem;
  border-radius: 50px;
  font-weight: 600;
  font-size: 0.9rem;
}

.detailed-features {
  background: white;
  padding: 4rem;
  border-radius: 20px;
  box-shadow: 0 20px 60px rgba(0,0,0,0.1);
  margin-bottom: 4rem;
}

.detailed-features h3 {
  text-align: center;
  font-size: 2.5rem;
  margin-bottom: 1rem;
  color: #1e293b;
}

.features-intro {
  text-align: center;
  font-size: 1.2rem;
  color: #64748b;
  margin-bottom: 3rem;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
}

.feature-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2.5rem;
  margin-top: 3rem;
}

.feature-item {
  padding: 2rem;
  border-radius: 15px;
  background: #f8fafc;
  transition: transform 0.3s ease;
}

.feature-item:hover {
  transform: translateY(-5px);
  background: white;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
}

.feature-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.feature-item h4 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #1e293b;
}

.feature-item > p {
  color: #64748b;
  margin-bottom: 1.5rem;
  line-height: 1.7;
}

.feature-sublist {
  list-style: none;
}

.feature-sublist li {
  padding: 0.5rem 0;
  color: #475569;
  padding-left: 1.5rem;
  position: relative;
}

.feature-sublist li:before {
  content: '•';
  position: absolute;
  left: 0;
  color: #667eea;
  font-weight: bold;
  font-size: 1.2rem;
}

.industry-solutions {
  background: white;
  padding: 4rem;
  border-radius: 20px;
  box-shadow: 0 20px 60px rgba(0,0,0,0.1);
  margin-bottom: 4rem;
}

.industry-solutions h3 {
  text-align: center;
  font-size: 2.5rem;
  margin-bottom: 3rem;
  color: #1e293b;
}

.industry-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.industry-card {
  text-align: center;
  padding: 2rem;
  border-radius: 15px;
  background: #f8fafc;
  transition: transform 0.3s ease;
}

.industry-card:hover {
  transform: translateY(-5px);
  background: white;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
}

.industry-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.industry-card h4 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #1e293b;
}

.industry-card p {
  color: #64748b;
  line-height: 1.6;
}

.benefits-section {
  background: white;
  padding: 4rem;
  border-radius: 20px;
  box-shadow: 0 20px 60px rgba(0,0,0,0.1);
}

.benefits-section h3 {
  text-align: center;
  font-size: 2.5rem;
  margin-bottom: 3rem;
  color: #1e293b;
}

.benefits-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2.5rem;
}

.benefit-item {
  text-align: center;
  padding: 2rem;
}

.benefit-number {
  font-size: 4rem;
  font-weight: 800;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 1rem;
  line-height: 1;
}

.benefit-item h4 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #1e293b;
}

.benefit-item p {
  color: #64748b;
  line-height: 1.7;
}

/* Pricing Section */
.features-grid {
  padding: 120px 0;
  background: white;
}

.section-header {
  text-align: center;
  margin-bottom: 4rem;
}

.section-header h2 {
  font-size: clamp(2.5rem, 5vw, 3.5rem);
  margin: 1.5rem 0;
  color: #1e293b;
}

.section-subtitle {
  font-size: 1.2rem;
  color: #64748b;
  max-width: 700px;
  margin: 0 auto;
  line-height: 1.7;
}

.pricing-cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
  margin-bottom: 3rem;
}

.pricing-card {
  background: white;
  padding: 3rem 2rem;
  border-radius: 20px;
  box-shadow: 0 20px 60px rgba(0,0,0,0.1);
  text-align: center;
  position: relative;
  transition: all 0.3s ease;
  border: 2px solid transparent;
}

.pricing-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 30px 80px rgba(0,0,0,0.15);
}

.pricing-card.popular {
  border: 2px solid #667eea;
  transform: scale(1.05);
}

.pricing-card.popular:hover {
  transform: scale(1.05) translateY(-10px);
}

.popular-badge {
  position: absolute;
  top: -15px;
  left: 50%;
  transform: translateX(-50%);
  background: linear-gradient(135deg, #ff6b6b 0%, #feca57 100%);
  color: white;
  padding: 0.5rem 1.5rem;
  border-radius: 50px;
  font-size: 0.9rem;
  font-weight: 600;
}

.pricing-card h3 {
  font-size: 1.8rem;
  margin-bottom: 1rem;
  color: #1e293b;
}

.price {
  font-size: 3.5rem;
  font-weight: 800;
  color: #1e293b;
  margin-bottom: 0.5rem;
}

.price span {
  font-size: 1rem;
  font-weight: 400;
  color: #64748b;
}

.price-description {
  color: #64748b;
  margin-bottom: 2rem;
  font-size: 0.95rem;
}

.pricing-card ul {
  list-style: none;
  margin-bottom: 2.5rem;
  text-align: left;
}

.pricing-card li {
  padding: 0.75rem 0;
  color: #64748b;
  border-bottom: 1px solid #f1f5f9;
}

.pricing-card li:last-child {
  border-bottom: none;
}

.trial-info {
  margin-top: 1rem;
  font-size: 0.85rem;
  color: #94a3b8;
}

.pricing-footer {
  text-align: center;
  padding-top: 2rem;
  border-top: 1px solid #e2e8f0;
  color: #64748b;
}

/* Testimonials */
.testimonials {
  padding: 120px 0;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
}

.testimonials .section-header h2 {
  color: white;
}

.testimonials .section-subtitle {
  color: rgba(255,255,255,0.9);
}

.testimonial-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
}

.testimonial-card {
  background: rgba(255,255,255,0.1);
  backdrop-filter: blur(10px);
  padding: 2.5rem;
  border-radius: 20px;
  border: 1px solid rgba(255,255,255,0.2);
  transition: transform 0.3s ease;
}

.testimonial-card:hover {
  transform: translateY(-5px);
  background: rgba(255,255,255,0.15);
}

.stars {
  color: #fbbf24;
  font-size: 1.5rem;
  margin-bottom: 1.5rem;
}

.testimonial-text {
  font-size: 1.2rem;
  font-style: italic;
  margin-bottom: 2rem;
  line-height: 1.7;
}

.author {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.avatar {
  width: 50px;
  height: 50px;
  background: rgba(255,255,255,0.3);
  border-radius: 50%;
  flex-shrink: 0;
}

.author-info {
  flex: 1;
}

.author-name {
  font-weight: 600;
  margin-bottom: 0.25rem;
}

.author-title {
  font-size: 0.9rem;
  opacity: 0.9;
}

/* CTA Sections */
.cta-section {
  padding: 100px 0;
  background: #f8fafc;
  text-align: center;
}

.cta-section h2 {
  font-size: 3rem;
  margin-bottom: 1rem;
  color: #1e293b;
}

.cta-section p {
  font-size: 1.3rem;
  color: #64748b;
  margin-bottom: 2.5rem;
}

.final-cta {
  padding: 120px 0;
  background: #1e293b;
  color: white;
  text-align: center;
}

.final-cta h2 {
  font-size: clamp(2.5rem, 5vw, 3.5rem);
  margin-bottom: 1.5rem;
}

.cta-subtitle {
  font-size: 1.3rem;
  margin-bottom: 2.5rem;
  opacity: 0.9;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
}

.cta-buttons {
  display: flex;
  gap: 1.5rem;
  justify-content: center;
  flex-wrap: wrap;
  margin-bottom: 3rem;
}

.cta-features {
  display: flex;
  gap: 2rem;
  justify-content: center;
  flex-wrap: wrap;
  margin-top: 3rem;
  padding-top: 3rem;
  border-top: 1px solid rgba(255,255,255,0.1);
}

.cta-feature {
  color: rgba(255,255,255,0.9);
  font-size: 1rem;
}

.cta-button.secondary.large {
  background: transparent;
  border: 2px solid #e2e8f0;
  color: white;
}

.cta-button.secondary.large:hover {
  background: rgba(255,255,255,0.1);
}

/* Footer */
.footer {
  background: #0f172a;
  color: #94a3b8;
  padding: 4rem 0 2rem;
}

.footer-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 3rem;
  margin-bottom: 3rem;
}

.footer-section h4 {
  color: white;
  margin-bottom: 1.5rem;
  font-size: 1.1rem;
}

.footer-section ul {
  list-style: none;
}

.footer-section li {
  margin-bottom: 0.75rem;
}

.footer-section a {
  color: #94a3b8;
  text-decoration: none;
  transition: color 0.3s ease;
}

.footer-section a:hover {
  color: white;
}

.footer-bottom {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 2rem;
  border-top: 1px solid #334155;
  flex-wrap: wrap;
  gap: 1rem;
}

.footer-social {
  display: flex;
  gap: 1.5rem;
}

.footer-social a {
  color: #94a3b8;
  text-decoration: none;
  transition: color 0.3s ease;
}

.footer-social a:hover {
  color: white;
}

/* Responsive Design */
@media (max-width: 1024px) {
  .image-section .container {
    grid-template-columns: 1fr;
    gap: 3rem;
  }

  .image-section.right .container {
    direction: ltr;
  }

  .content-grid {
    grid-template-columns: 1fr;
  }

  .pricing-card.popular {
    transform: scale(1);
  }

  .pricing-card.popular:hover {
    transform: translateY(-10px);
  }
}

@media (max-width: 768px) {
  .hero {
    height: 90vh;
    min-height: 500px;
  }

  .hero-headline {
    font-size: 2.5rem;
  }

  .hero-stats {
    gap: 2rem;
  }

  .stat-number {
    font-size: 2rem;
  }

  .image-section,
  .long-content,
  .features-grid,
  .testimonials,
  .cta-section,
  .final-cta {
    padding: 80px 0;
  }

  .image-content h2,
  .content-header h2,
  .section-header h2 {
    font-size: 2rem;
  }

  .feature-grid,
  .industry-grid,
  .benefits-grid {
    grid-template-columns: 1fr;
  }

  .pricing-cards {
    grid-template-columns: 1fr;
  }

  .testimonial-grid {
    grid-template-columns: 1fr;
  }

  .cta-buttons {
    flex-direction: column;
    align-items: stretch;
  }

  .cta-button.large {
    width: 100%;
  }

  .footer-content {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .footer-bottom {
    flex-direction: column;
    text-align: center;
  }

  .detailed-features,
  .industry-solutions,
  .benefits-section {
    padding: 2rem;
  }

  .content-block {
    padding: 2rem;
  }
}

@media (max-width: 480px) {
  .container {
    padding: 0 15px;
  }

  .hero {
    height: 85vh;
  }

  .hero-cta {
    flex-direction: column;
  }

  .cta-button {
    width: 100%;
  }

  .content-metrics {
    flex-direction: column;
  }

  .metric {
    text-align: center;
  }

  .cta-features {
    flex-direction: column;
    gap: 1rem;
  }
}
</style>