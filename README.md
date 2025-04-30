# Setup

1. Install Ruby 3.3 (https://www.ruby-lang.org/en/)
2. Install gems:
   ```
   bundle install
   ```
3. Install prettier and prettier-plugin-tailwindcss:
   ```
   npm install
   ```

# Demo

1. Run development server
   ```
   bin/dev
   ```
2. Visit localhost:3000 and see working tailwind with prefix
3. Format the shown html with prettier
   ```
   npm exec prettier app/views/home/show.html
   ```
4. See that classes without prefix get sorted but the ones with prefix do not

   ```
   <div class="tw:bg-red-300 tw:size-20">prefix</div>
   <div class="tw:size-20 tw:bg-blue-300">prefix</div>

   <div class="size-20 bg-red-300">no prefix</div>
   <div class="size-20 bg-blue-300">no prefix</div>
   ```
