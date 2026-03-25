---
applyTo: '**'
---

# SSC CGL Question Paper Generator - Comprehensive AI Development Guidelines

## Project Overview
This repository contains a specialized educational content generator designed to create comprehensive HTML-based question papers for exam preparation. The project focuses on various topics, and generates self-contained, printer-friendly documents with detailed solutions in Hindi.

## Architecture & Project Structure

### Repository Organization
```
Question papers/
├── .github/
│   ├── instructions/
│   │   └── instructions.instructions.md    # This file - AI guidelines
│   ├── prompts/
│   │   └── Ques.prompt.md                  # Content generation templates
│   └── copilot-instructions.md             # GitHub Copilot specific guidelines
├── Simple_Interest_SSC CGL_Practice_Set.html   # Example question paper
└── [Future topic files].html               # Additional subject matter
```

### Core Components Analysis

#### 1. HTML Question Papers
**Structure Pattern**: Self-contained documents with embedded styling
- **Language**: Hindi (Devanagari script) with `lang="hi"` attribute
- **Format**: Complete HTML5 documents with embedded CSS
- **Content**: 30 standardized multiple-choice questions with detailed solutions
- **Styling**: Print-optimized responsive design with clean typography

#### 2. Content Architecture
Based on `Simple_Interest_SSC CGL_Practice_Set.html` analysis:

**Header Section**:
```html
<h1>प्रैक्टिस सेट (परीक्षा)</h1>
```

**Question Format**:
```html
<div class="question" id="q1">
    <p>1. [Hindi question text with mathematical content]</p>
    <ul class="options">
        <li>(A) Option 1</li>
        <li>(B) Option 2</li>
        <li>(C) Option 3</li>
        <li>(D) Option 4</li>
    </ul>
</div>
```

**Solution Format**:
```html
<div class="solution" id="s1">
    <p><strong>1. हल (B)</strong></p>
    <p>[Step-by-step explanation in Hindi]</p>
    <p>[Mathematical calculations]</p>
    <p>[Final answer with reasoning]</p>
</div>
```

## Technical Implementation Standards

### HTML Structure Requirements
1. **Document Declaration**: HTML5 with Hindi language specification
2. **Meta Tags**: UTF-8 charset and responsive viewport
3. **Semantic Structure**: 
   - Container-based layout (`<div class="container">`)
   - Question sections with unique IDs (`id="q1"`, `id="q2"`, etc.)
   - Solution sections with corresponding IDs (`id="s1"`, `id="s2"`, etc.)
4. **Accessibility**: Proper heading hierarchy and semantic markup

### CSS Design System
Based on the existing implementation:

**Core Layout**:
```css
.container {
    max-width: 800px;
    margin: auto;
    background: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
```

**Typography & Styling**:
- Font: Arial sans-serif for Hindi readability
- Color scheme: Dark text (#333) on light backgrounds
- Accent colors: Blue theme (#2c3e50, #3498db)
- Line height: 1.6 for optimal readability

**Print Optimization**:
```css
@media print {
    .solutions { page-break-before: always; }
    .question, .solution { page-break-inside: avoid; }
}
```

### Content Standards & Guidelines

#### Mathematical Content Requirements
1. **Currency**: Use ₹ symbol consistently for Indian Rupee
2. **Mathematical Notation**: Standard symbols (×, ÷, %, =, etc.)
3. **Formula Presentation**: Clear step-by-step derivations
4. **Calculations**: Show all intermediate steps in solutions

#### Language & Localization
1. **Primary Language**: Hindi (Devanagari script)
2. **Mathematical Terms**: Use standard Hindi mathematical terminology
3. **Number Format**: Indian numbering system with appropriate separators
4. **Cultural Context**: Real-world scenarios relevant to Indian context

#### Question Paper Specifications
Based on `Ques.prompt.md` and existing content:

1. **Question Count**: Exactly 30 questions per topic
2. **Question Types**:
   - Basic calculation problems
   - Word problems with real-world scenarios
   - Application-based questions
   - Tricky calculations requiring logical reasoning
3. **Difficulty Distribution**: Mixed difficulty levels appropriate for SSC CGL exam level
4. **Answer Format**: Multiple choice with 4 options (A-D)
5. **Solution Requirement**: Detailed step-by-step explanations for each question

## Development Workflows & Best Practices

### Creating New Question Papers
1. **Template Usage**: Copy structure from `Simple_Interest_SSC CGL_Practice_Set.html`
2. **Content Generation**: Use `.github/prompts/Ques.prompt.md` as reference
3. **Quality Validation**:
   - Verify mathematical accuracy
   - Check Hindi grammar and terminology
   - Test print layout functionality
   - Validate HTML structure

### File Naming Conventions
- Question papers: `{Subject}_SSC CGL_Practice_Set.html`
- Prompt templates: `{Purpose}.prompt.md`
- Instruction files: `{Context}.instructions.md`

### Code Quality Standards
1. **HTML Validation**: Must be valid HTML5
2. **CSS Organization**: Embedded styles with logical grouping
3. **Content Accuracy**: Mathematical correctness verified
4. **Responsive Design**: Mobile and print compatibility
5. **Performance**: No external dependencies for offline usage

## Integration & Deployment Considerations

### Browser Compatibility
- Target: Modern browsers with print functionality
- Print-to-PDF: Optimized for browser-based PDF generation
- Mobile: Responsive design for various screen sizes

### Accessibility Features
- Semantic HTML structure
- Proper heading hierarchy
- High contrast text for readability
- Print-friendly layouts

### Maintenance Guidelines
1. **Content Updates**: Regular review of question relevance
2. **Template Evolution**: Maintain consistency across files
3. **Style Consistency**: Unified design language
4. **Documentation**: Keep instructions current with implementation

## AI Development Guidelines

### When Creating New Content
1. **Research Phase**: Understand syllabus requirements
2. **Content Planning**: Ensure comprehensive topic coverage
3. **Implementation**: Follow established HTML/CSS patterns
4. **Validation**: Test mathematical accuracy and formatting
5. **Optimization**: Verify print and mobile compatibility

### Code Generation Principles
1. **Consistency**: Maintain established patterns and conventions
2. **Quality**: Prioritize accuracy over speed
3. **Accessibility**: Consider diverse user needs
4. **Performance**: Optimize for fast loading and printing
5. **Maintainability**: Write clear, documented code

This comprehensive guide ensures consistent, high-quality output aligned with the project's educational objectives and technical requirements.