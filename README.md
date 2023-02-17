# QuickHull-DivideAndConquer

PenguHull - Tales of a (very) drunk Penguin

Global warming is affecting penguins. After extensive analysis, the excellently studied penguins of the PUM have determined that they have to start keeping farm animals in order to ensure
sufficient food. Since penguins prefer to eat fish, they very quickly agreed that they wanted to mark off an area in the water in order to breed the fish there and then be able to catch them more
easily. Fortunately, the researchers have been creating elaborate maps for generations to know where the schools of fish are usually located. In order to have fish in your breeding right from the
start, you now want to set up a fence in the water around a group of such positions and start breeding.
In a survey, the researchers have already determined which shoals of fish taste the best and one thing is certain: we can start breeding the tastiest fish tomorrow! … (A PinguUniParty at the Irish
Pub later) … Oh jeh! The overzealous penguin Max seems to have drunk one Guinness too much. Max has haphazardly anchored all of the existing stakes into the seabed and there is no way to
get them out again. There is only one option: we need to build the fence along the already set stakes. But how do we fence in the largest possible area with the existing posts? Surely you can
write a program to find out. Or?

Explanation:
In this issue we will develop a program together to calculate approximately convex hulls. In order to reduce the mathematical complexity, the specification is kept quite informal. So if you want
to learn more about the subject, or prefer mathematical definitions, you're welcomehere (Convex Hulls of Finite Sets of Points in Two and Three Dimensions - Maximilian Anziger)check. If there is
enough interest, there will also be a dedicated (special) PGdP coffee party.
You can imagine the problem formulated above as a board full of nails. The solution we're looking for is equivalent to what would happen if you put a rubber band around ALL the nails.

Presentation of points/point listings:
Points and listings of points are presented in our program as follows:
One point(x,y)is represented by an integer array with two entries:{x, y}. The entry 0 corresponds to the x-coordinate and the entry 1 to the y-coordinate.
A collection (a set, so to speak - except that they occur in a fixed order and there may be duplicates) of multiple points is represented as a 2D array (oftenint[][] points) shown. The inner
arrays all have two entries and represent the individual points in the manner just described.

Launch:
Implement the methodint[][] quickHull(int[][] points). This method receives an array of the coordinates of all posts ({{x0, y0}, {x1, y1}, ...}) with which you should delimit the area. Returns the convex
hull with the leftmost point inpoints(the one fromfindLeftmostPoint(points)is returned) as the starting point. So this is a closed shell. Also look for the rightmost point inpointsand then start the
algorithm with appropriate calls to quickHullLeftOf().

Full project description with visual representation in project_description.pdf
