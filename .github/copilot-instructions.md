# UPSI Question Paper Generator - AI Coding Guidelines

## Project Overview
This repository creates educational HTML documents for UPSI (Uttar Pradesh Police Sub Inspector) exam preparation, specifically focusing on mathematical topics like Simple Interest. The project generates printer-friendly question papers in Hindi with comprehensive solutions.

## Architecture & Structure

### Core Components
- **HTML Question Papers**: Self-contained documents with embedded CSS styling (`Simple_Interest_UPSI_Practice_Set.html`)
- **Prompt Templates**: AI generation instructions in `.github/prompts/` directory
- **Instructions**: Project-wide AI guidelines in `.github/instructions/`

### Content Structure Pattern
All question papers follow this standardized format:
1. **Header**: Hindi title with subject and exam type
2. **Question Section**: 30 numbered questions with 4 multiple-choice options (A-D)
3. **Solutions Section**: Detailed step-by-step explanations in Hindi

## Technical Conventions

### HTML Structure Standards
- Use semantic HTML5 with `lang="hi"` for Hindi content
- Embed CSS in `<style>` tags (no external stylesheets)
- Question containers use `id="q1"`, `id="q2"` etc.
- Solution containers use `id="s1"`, `id="s2"` etc.
- Options formatted as unordered lists with class `options`

### CSS Design Patterns
```css
/* Container-based responsive design */
.container { max-width: 800px; margin: auto; }

/* Print-optimized styles */
@media print {
    .solutions { page-break-before: always; }
    .question, .solution { page-break-inside: avoid; }
}
```

### Content Guidelines
- **Language**: All content in Hindi (Devanagari script)
- **Currency**: Use ₹ symbol for Indian Rupee
- **Math Notation**: Use standard mathematical symbols (×, ÷, %, etc.)
- **Question Numbering**: Sequential 1-30 format
- **Option Labels**: (A), (B), (C), (D) format

## Development Workflows

### Creating New Question Papers
1. Copy the existing HTML structure from `Simple_Interest_UPSI_Practice_Set.html`
2. Update the title and subject matter
3. Replace questions while maintaining the 30-question format
4. Ensure each question has exactly 4 options
5. Provide detailed Hindi solutions with step-by-step calculations

### Using AI Prompts
- Reference `.github/prompts/Ques.prompt.md` for content generation guidelines
- Ensure generated content covers "basic calculations, word problems, application-based questions, scenarios"
- Include "tricky calculations and real-life applications"
- Maintain varied difficulty levels appropriate for UPSI exams

### Quality Standards
- Verify mathematical accuracy in both questions and solutions
- Ensure proper Hindi grammar and mathematical terminology
- Test print layout using browser print preview
- Validate HTML structure and CSS responsiveness

## File Naming Conventions
- Question papers: `{Subject}_UPSI_Practice_Set.html`
- Prompt files: `{Purpose}.prompt.md`
- Instruction files: `{Context}.instructions.md`

## Integration Points
- Browser print functionality for PDF conversion
- Mobile-responsive design for various screen sizes
- No external dependencies (self-contained HTML files)

## Mathematical Content Standards
- Use proper Hindi mathematical terminology
- Include formula derivations in solutions
- Show intermediate calculation steps
- Reference standard UPSI syllabus topics
