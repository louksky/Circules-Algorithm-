# Circules-Algorithm-
c# 2 simple for bersineaim check my repos
 //פונקצייה לציור מעגל מסתמכת על גבי שתי נקודות 
        //מרכז ורדיוס
        //שיטה ראשונה רקורסיבית 
        //!!!!! השתמשנו במימוש של ברזנהיים 
        
        
        
        {{{{
        double delta_1;
        double delta_2;
        double SIZE = 100;
        private void HelpRec_mycircule(Point N, Point C, double Q, double rq)
        {
            //חישוב ערכים טריגונמטרים פעם אחת 
             delta_1 = Math.Cos(Q);
             delta_2 = Math.Sin(Q);
              rec(N, C, 0);

        }
        private void rec(Point N, Point C, double rqcount )
        {
            if (rqcount >= SIZE) return;
            
            double x = C.X + N.X * delta_1 - N.Y * delta_2;
            double y = C.Y + N.Y * delta_1 + N.X * delta_2;

            PixelSet(new Point(x, y));

            rec(N, C, 1 + rqcount);

        }
        //private void myCirculeDraw(Point a, Point b)
        //{
        //    double y    ;
        //    double x    ;

        //    r = Point.Subtract(a, b).Length;
            
           
        //    RecursiveCircule(0, a ,2.6);
        //}
        //int deg = 180;
        //double r = 0;
        //private void RecursiveCircule(double i,Point p,double freq)
        //{
        //    if (i >= 360) return;

        //    double delta = i;
        //    double x = r * Math.Cos(delta * Math.PI / deg);
        //    double y = r * Math.Sin(delta * Math.PI / deg);
            
        //    PixelSet(new Point(p.X + x, y + p.Y));

        //    RecursiveCircule(i + freq, p, freq);

        //}
        private void MyCurve(Point[] points_array)
        {



        }
