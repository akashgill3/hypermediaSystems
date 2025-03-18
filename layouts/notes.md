Key Points in This Layout
Body Classes:
bg-gray-50 and text-gray-800 for a light background and dark text.
min-h-screen to ensure it stretches to the full viewport height.
Container & Spacing:
max-w-7xl mx-auto px-4 py-8 for a centered layout with horizontal and vertical padding.
Responsive Grid:
Top row uses grid grid-cols-1 md:grid-cols-3 gap-4 to stack widgets on smaller screens and place them in three columns on medium screens and up.
The main section below is split into two columns on medium screens (md:grid-cols-12), with the left column spanning 8 columns and the right column spanning 4 columns. On small screens, they stack (grid-cols-1).
Widget Styling:
Each widget is wrapped in bg-white rounded shadow p-4 to give a white card-like appearance with rounded corners, a drop shadow, and some internal padding.