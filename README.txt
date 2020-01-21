OR-Tools - Sudoku Solver - 

Ce code impl�mente une classe nom� : OrToolsSolver
et implemente l'interface : ISudokuSolver

pour r�soudre un sudoku il suffit d'appeler la m�thode : 

Sudoku Solve(Sudoku s)

cette m�thode retourne le sudoku r�solu. 

Exemple: 
	int[] initial_grid = new int[] { 0, 6, 0, 0, 5, 0, 0, 2, 0,

                                             0, 0, 0, 3, 0, 0, 0, 9, 0,

                                             7, 0, 0, 6, 0, 0, 0, 1, 0,

                                             0, 0, 6, 0, 3, 0, 4, 0, 0,

                                             0, 0, 4, 0, 7, 0, 1, 0, 0,

                                             0, 0, 5, 0, 9, 0, 8, 0, 0,

                                             0, 4, 0, 0, 0, 1, 0, 0, 6,

                                             0, 3, 0, 0, 0, 8, 0, 0, 0,

                                             0, 2, 0, 0, 4, 0, 0, 5, 0 };
	//cr�ation d'un sudoku 
 	Noyau.Sudoku s = new Noyau.Sudoku(initial_grid);
        Console.WriteLine(s.ToString());
	
	//cr�ation du solveur
        OrToolsSolver ORT = new OrToolsSolver();
        s = ORT.Solve(s);
        Console.WriteLine(s.ToString());


cette m�thode prend en param�tre un objet Sudoku qui permet de g�n�rer un sudoku.
cf:README de la classe Sudoku



